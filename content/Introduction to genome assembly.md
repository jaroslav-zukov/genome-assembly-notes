Every living organism has set of genetic instructions encoded in a long chain of DNA molecules. It's very practical to know the full DNA sequence of an organism, because of biological and evolutionary insight as well as perspectives for disease prediction and treatment.

DNA is composed from two strands of polynucleotides that coil around each other, forming a double helix 🧬. There are only 4 building blocks of DNA, nucleic bases, referred to as *A*, *T*, *G*, *C*. The size of the human reference genome is 3.2 billion base pairs (bp), the fruit fly genome is 180 million bp (Mbp) long and yeast has 12 Mbp. 

Okay, let's say we have yeast sample, how do we read its DNA sequence? In general we want some machine to read the longest possible stretches of DNA that would be as accurate as possible (100% read precision). There are multiple [[DNA sequencing technologies]] that attempt to do so. Usually one uses a combination of multiple technologies to overcome the drawbacks of each single technology. At the end once receives a collection of sequences of various lengths between 150 and 30000 bp with some read errors in them.

The classical way to state **genome assembly problem**: Having large amount of substring we want to reconstruct the original sequence. Or we can restate the problem in a slightly different way - How do we reconstruct the whole genomic sequence from the sequencing data?
![[Pasted image 20240709162203.png]]

What I describe here is so called *de-novo* assembly, which is the process of reconstructing the initial DNA sequence without the reference genome of a similar sample (same species).