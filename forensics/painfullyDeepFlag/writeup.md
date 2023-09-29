# painfullyDeepFlag - forensics


## Description
This one is a bit deep in the stack.
file: https://amateurs-prod.storage.googleapis.com/uploads/f80e99a7a081fa3fd0af3ae292ae8aeb0aa3e58dd053db6ba7c7a6162f0dc11a/flag.pdf

## Quick overview
So we have a pdf file, no interresting strings or metadata, we can analyse the objects included in the file

## Solution
First, we will take a look at the pdf file using `peepdf` to analyse the objects of the files looking for embeded files or hidden scripts
Actually that was the first idea, but nothing is found
Then I tried to convert the pdf to other format maybe there is data that can be clear in other format
I used `pdftohtml` then welcome dear flag: `amateursCTF{0ut_0f_b0unds}`

