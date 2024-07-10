---
title: Home
---
## Introduction
Genome assembly is a flagship problem in bioinformatics. There are plenty of large-scale projects focused on sequencing many de novo genomes from all walks of life. Even though we were able to assemble a whole human genome, it is still a very costly and complex problem for which we haven't a single and efficient solution.

We propose a radically new approach to this problem. Instead of collecting several sources, converting them into strings and then creating a superstring, we want to take raw signals produced by Oxford Nanopore sequencers and create raw signal assembly, which can be converted into nucleotide sequence at the very end.

![[Pasted image 20240710114143.png]]

### Proposed approach
1. Sequence the DNA with Oxford Nanopore (Generate Nanopore signal)
2. Run discrete Fourier transform on the nanopore signal (Reads → $\mathbb{R}^n$ )
3. Convert the reads in $\mathbb{R}^n$ into geometric inhomogeneous random graph ([[GIRG]])
	1. Represent each read in a vertex
	2. Apply the *distance* function that calculates overlap quality of signals
	3. Assign the probability of an edge to the *distance* between two nodes
4. Extract a couple of most probable graphs with certain properties
	1. There exists a hamiltonian cycle of certain length (T2T assembly is possible)
	2. The cycle preserves a coverage (each base is read approximately same number of times)
5. Extract the most probable hamiltonian path (raw assembled T2T signal)
6. Basecall and validate the assembly (or compare them with other assemblies)

The implementation should be done end-to-end, massively parallelizable and designed to run on a GPU clusters (it has just more FLOPS).

Proposed approach would work only in the case if following **assumption** holds:
> [!question]-   Same DNA regions must produce very similar signal waves

### Advantages
The process of basecalling is *lossy* in nature, and also it's hugely biased on the human data - it has larger basecall error on fish and invertebrates because of the training dataset for the basecalling models. We take in consideration much more information about the read - context of the neighboring nucleotides and chemical modifications. We are also agnostic to the pore chemistry - the algorithm will work with a new pore type. The only constraint is the consistency of the pore chemistry for one assembly (because same reads have to produce very similar signals)

## Plan of action
1. Verify assumptions
2. Construct the theoretical solution + build the proof of concept
	1. Find a distance function for finding overlaps from DFT transformed waves
	2. Research how exactly can we apply [[GIRG]]s - theoretical solution
		1. encoding of $\mathbb{R}^n$ into the graph with the distance function
		2. finding the most probable graphs
	3. Try to create a unified end-to-end theoretical framework
3. Collect a team of experienced engineers and build the thing using software best practices


___
For more context:
- What is genome assembly? → [[Introduction to genome assembly]]
- Why do you do that? → [[Motivation]]
- Large-scale sequencing projects → [[Sequencing initiatives]]
- Our ideas → [[Ideas for the new assembler]]
- Who are you? → [[About me]]

Side things:
- [[My Questions]]
