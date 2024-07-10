Ultimately I want to build new genome assembler that would 
1. use exclusively Oxford Nanopore data (of one cell for one assembly)
2. drop the legacy limitations
3. Use newest graph theory theorems
4. be massively parallel - on GPU
5. be an end-to-end process

The genome assembly (or even *de novo*) is very ambitious task, which shouldn’t be tackled by one person, otherwise it would took ages. But rather I should build a strong team of mathematicians, software engineers and biologists, who would be able to deliver biologically relevant, highly (algorithmically) optimized, clean and scalable code iteratively and quickly.

### Practical Goal - Assemble my sequence
It would be cool to assemble my own genome with the newly developed assembler and nanopore data.

Why am I doing this?
### Bachelor thesis idea
- collecting and summarizing information on the genome assembly problem
	- end to end overview, historical context
- formally diving into the algorithms used
	- is there a room for improvement?
	- collaborating with Panagiotou on the algorithms
- code implementation
	- review of current solutions
	- writing a new one
		- applying massive parallelism to the approach ([[bend]])

