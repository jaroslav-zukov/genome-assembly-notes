Before the each phase define a clear SMART goals and schedule a report presentation with people interested.
### 1. Getting started - 2 weeks
Run simple assembly, visualize and benchmark resulting assembly graphs
	- [[Verkko]]
	- [[Hifiasm]]
	- [[Flye]]
Create a short overview/presentation/description of the inner workings and computational complexity of those solutions. How the computational resources are utilized?

### 2. Proof of concept - FFT and distance function - 1 week
Create a synthetic pipeline which will assemble the signal function with added distortion on top of it. Here's the rough overview of the steps needed
1. Create synthetic signal ($\mathbb{R} \rightarrow \mathbb{R}$  function)
2. Slice and distort the signals in the different ways
	1. predictable slicing - constant coverage
	2. First try with clean signal
	3. Add the small noice on top, play with noice intensity
3. Reconstruct the original signal (use overlap brute force approach)
	1. FFT the signal
	2. Find the overlap probability and size

### 3. Proof of concept - Random graphs and hamiltonian cycles - 2 weeks 
Research the idea of encoding the overlap distances into the edge probabilities, visualizing and assessing the assembly. Use synthetic data.
Try to implement [[GIRG]] solution and find a most probable hamiltonian cycles in them. 

Don't think about computational complexity and parallelism at this point.

### 4. Finalize theoretical approach and analyze complexity - 1 week
Create an end-to-end theoretical description for going from raw reads to the assembly. Analyze the computational complexity and opportunities for parallelism

### 5. Start with the implementation
Create a team of engineers, mathematicians and biologists to implement the solution.