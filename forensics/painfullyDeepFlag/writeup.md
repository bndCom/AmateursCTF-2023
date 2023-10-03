# painfullyDeepFlag - forensics


## Description
This one is a bit deep in the stack.
file: https://amateurs-prod.storage.googleapis.com/uploads/f80e99a7a081fa3fd0af3ae292ae8aeb0aa3e58dd053db6ba7c7a6162f0dc11a/flag.pdf

## Quick overview
We have a PDF file devoid of interesting strings or metadata, prompting us to analyze the embedded objects within it.

## Solution
Our initial approach involved using `peepdf` to scrutinize the PDF's objects, searching for hidden scripts or embedded files. However, this yielded no results.
Subsequently, we attempted to convert the PDF into other formats, hoping to uncover hidden data. We employed `pdftohtml`, and to our delight, we discovered the following flag: `amateursCTF{0ut_0f_b0unds}`.

