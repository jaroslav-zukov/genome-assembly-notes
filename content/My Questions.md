>[!Warning]- DRAFT

What do I want to know about existing approaches?

What do I want to learn for my attempt


## Existing approaches

### Implementational questions
-  How have people solved the assembly problem before?
- what are the best assemblers at the time and how do they work
	- what algorithms are used
	- what are the steps - from start to finish
	- what are the tricks and ideas used
	- what are their limitations
- what are the main ideas used in different assemblers
	- create a high level mind map of ideas

### Theoretical questions
- What’s the computational complexity of existing genome assembly algorithms/programs? - answer in big O notation
- What is the mathematics behind existing genome assembly algorithms
	- write about that - maybe bachelor thesis
- How does de novo assembly works?
	- why is that much harder than with the reference genome?
	- how does assembly with the reference genome works?

### Computational questions
- Can the process of the assembly be parallelized on the modern GPU?
- [[Estimation of assembly computational complexity on a GPU node]]
- How long does it take to perform assembly on a GPU?
	- Answer: Assuming there are no computational bottlenecks, the computational complexity with n plugged inside.

## My approach

### Theory
How could recent theoretical advancements in following disciplines be integrated into my solution?

- graph theory
	- random graphs + hamiltonian paths + efficient algorithms
	- state the problem in the different theoretical framework
		- some probabilistic graph with certain properties
		- custom mathematical object highly optimized for the end-to-end genome assembly
- computer science
	- parallel computing
	- data structures
	- machine learning? Graph neural networks?
- Signal processing - functional analysis - do some research on following
	1. Fourier transform or alternatively (suggested by GPT)
	2. Dynamic Time Warping (DTW)
	3. Cross-Correlation
	4. Fourier Transform and Phase Correlation
	5. Hidden Markov Models (HMMs)
	6. Wavelet Transform
	7. other stuff
		1. Short-Time Fourier Transform (STFT)
		2. Hilbert Transform
		3. Z-Transform
		4. Principal Component Analysis
		5. Empirical Mode Decomposition
		6. Time-Frequency Distribution (Wigner-Ville Distribution)
		7. Autoregressive (AR) and Autoregressive Moving Average (ARMA) Models
		8. Kalman Filter
		9. Nonlinear Time Series Analysis (Recurrence Plot)