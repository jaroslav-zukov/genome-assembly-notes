>[!Warning]- DRAFT

## Theory
If we were to encode the reads with an distance/similarity function into an overlap random graph by changing the probabilities of specific edges, than we could receive something similar to a lossless representation of the reads inside the graph space. And in that weighted graph space we could then search for a specific properties, like a hamiltonian path with an even coverage.

Maybe we could even encode some biological or technical artifacts inside the weights

### Graph theory
Is there a more effective representation of the data?
	1. Can we use a structure of a random graph? 
		1. give some conditions at the start
		2. look for the most attractive possibilities given the search across all possible graphs
	2. It would be great to encode the proximity/similarity of the reads directly into the graph


### Signal processing
2. Try using bend implement graph algorithms of the assembly
	1. start small - with individual algorithms
4. If we were to use only nanopore, do we have to basecall before alignment? Doesn’t it strip the information away?
	1. try aligning the raw reads or in some intermediary form - together with modifications
	2. can we find the similarity of the squiggles effectively? maybe there is some hard math involved - signal level processing - similarity function
	3. Also we need to somehow overlay simplex nanopore reads to the ultra-long ones, which also needs a conversion function


## Practice
### Paralelism
Use programming language with a support of parallel computing. Here are a couple of candidates:
- Bend
- Mojo
- Rust
- C++

### Signal processing
Can some conversion be done already on the hardware level? Like when reading from a sequencing device? Can we leverage Digital signal processors for this?
