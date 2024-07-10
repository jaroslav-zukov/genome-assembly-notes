---
title: Home
---
## Intro and high level overview
Genome assembly is a flagship problem in bioinformatics. There are plenty of large-scale projects focused on sequencing many de novo genomes from all walks of life. Even though we were able to assemble a whole human genome, it is still a very costly and complex problem for which we haven't a single and efficient solution.

We propose a radically new approach to this problem. Instead of collecting several sources, converting them into strings and then creating a superstring, we want to take raw signals produced by Oxford Nanopore sequencers and create raw signal assembly, which can be converted into nucleotide sequence at the very end.

![[Pasted image 20240710114143.png]]

The approach consists of
1. Sequence the DNA with Oxford Nanopore (Generate Nanopore signal)
2. Run discrete Fourier transform on the nanopore signal (Reads → $\mathbb{R}^n$ )
3. Convert the reads in $\mathbb{R}^n$ into inhomogeneous random geometric graph
	1. Represent each read in a vertex
	2. Apply the *distance* function that calculates overlap quality of signals
	3. Assign the probability of an edge to the *distance* between two nodes
4. Extract a couple of most probable graphs with certain properties
	1. There exists a hamiltonian cycle of certain length (T2T assembly is possible)
	2. The cycle preserves a coverage (each base is read approximately same number of times)
5. Extract the most probable hamiltonian path (raw assembled T2T signal)
6. Basecall and validate the assembly 

___
For more context:
What is genome assembly? → [[Introduction to genome assembly]]
Why do you do that? → [[Motivation]]
Large-scale sequencing projects → [[Sequencing initiatives]]
Our ideas → [[Ideas for the new assembler]]
Who are you? → [[About me]]

Side things:
- [[My Questions]]
