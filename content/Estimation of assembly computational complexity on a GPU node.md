**Goal**: estimate the complexity of the assembly algorithm

If we were to set an arbitrary maximum time of a genome assembly, let’s say 4 hours. Multiply this time by the computing power or modern GPU clusters.

Let’s assume that we’re going to run the assembly on one *NVIDIA DGX H100* node.
So one GPU node provides 32 petaflops, which makes the formula
$$
4h \times 32 \text{ petaflops} = 1.44*10^4s \times 3.2*10^{16} \text{ op/s} = 4.608*10^{20} \text{operations}
$$
Let’s be conservative with the coverage, let’s say we would have 30x coverage (even though I think less coverage would also get the job done). Given that the human genome is 3.2Gb, the average nanopore read is 20kb long we would have
$$
\frac{3.2Gb}{20kb}*30 = \frac{3.2*10^9}{2*10^3}*30=4.8*10^7 \text{ reads}
$$
So we need to design an algorithm with a complexity between quadratic and cubic complexity, $O(n^{2.69})$ to be exact. Which is a lot, and that's only one node which costs $2.49/hr on lambdalabs at the moment (9.7.2024).

Maybe it’s also helpful to think in terms of the individual nucleotides, because they introduce the squiggle pattern, but I don’t know how to calculate that exactly.