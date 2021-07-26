Some of my notes from Andrej Karpathy's Article on Medium <a href="https://karpathy.medium.com/software-2-0-a64152b37c35">here</a>

Software 2.0

Neural Networks = Software 2.0

Software 1.0 consists of explicit instructions written in C++, Python etc

2.0 consists of “weights” or probabilities, not a human friendly language
	Specify some goal on the behavior of a desirable out come 
	Create a data set of input out put pairs

The Neural Net Architecture is still explicitly written as the “skeleton”of the code 
	it Identifies a subset of program space to search
		the search can be optimized with back propagation and stochastic gradient descent

Back Propagation 
	can be thought of as a class of algorithms
	computes the gradient of the loss function with respect to the weight of a single input output pair.
	this is an example of dynamic programming

Gradient 
	In vector calculus it is the gradient of Scalar-value differential function of several variables
	Its is represented as a vector field

Loss Function
	function that maps values into a real number intuitively representing the “cost” of an event

Dynamic Programming
	mathematical optimization method and a computer programming method
	simplifies a complex problem into simpler sub problems in a recursive manner. 

1.0 consists of human engineered code that compiles into binary
2.0 consists of the data set that defines desirable behavior &
			the network architecture
	the weights are all filled in by the model
	this data set is compiled into binary

*Neural Network Architectures and training systems are increasingly standardized into a commodity.
		?Is this like Tensor Flow and PyTorch?
So, 2.0 software development is mostly curating, growing, massaging and cleaning labeled data sets
	?how does this relate to MuZero or Open Pilot?
	?What does Hotz mean by saying everything will be “end to end ML”?

1.0 Maintains surrounding training code, infrastructure, analytics, visualizations and labeling interfaces 

Common theme in software is to convert code bases to 2.0 and or even solve novel problems with 2.0, giving up on 1.0. 

use cases:
Visual Recognition 
Speech Recognition 
	Gaussian Mixture Model
		Statistical probabilistic model for predicting sub populations in a larger population. No observed data set is needed to identify the sub pop
	Markov Models
		Stochastic model of pseudo random changing systems.  Future state is only dependent on current state. 
Speech Synthesis
	ConvNets Like WaveNet
Machine Translation 
Games
	like AlphaGo
Data Bases
	Replaces traditional data management systems, out performing cache optimized B-trees
	B-tree is a self balancing data structure.

Convolutional Neural Networks (ConvNets)
	class of deep neural networks
	commonly used to analyze visual imagery
	regularized versions of multi layer perceptrons
	modeled after the visual cortex in the brain
	less pre processing when compared to image classification algorithms
	optimizes filters through automated learning
	 “hallucinating” images, sounds, and text with generative models

"One Model to rule them all”

Computationally Homogenous 
	NN’S are primarily 2 operations 
		Matrix multiplication & thresholding at zero (ReLU)
	Thresholding 
		Separate out regions of an image to analyze, i.e.: differentiate pixels 
	..Classical software is more heterogeneous and complex. 

Instruction set of a NN is relatively small, implementation is “much closer to silicon” especially with ASICS and Neuromorphic chips.
	neuromorphic chips are meant to mimic neuro biological architectures

Constant Run Time
	all NN foreward passes take the same amount of flops, there is no complex path through large codebases. 
	no need for dynamic compute graphs
	less likely to be caught in infinite loops
 
Memory Use
	There is no dynamically allocated memory, low possibility of swapping to disk.

Portable
	Sequence of matrix multiplies is significantly easier to run on arbitrary configurations as compared to binaries to scripts. 

Agility
	Easy to modify is runtime at cost of performance. Simply remove channels. channels are essentially all made of the same architecture. The same ease of use is true for adding channels with more data.

Limitations	

Explainability
	At the end of the optimization it is hard to tell how they work. 
	this is an ongoing topic in ai (clarity).
	Silently adopt biases

Takeaway
	2.0 can be viewed as another tool within 1.0 (NN’s) or can be understood as a whole new paradigm in itself (essentially what Karpathy argues).
	There remains much work to be done to support the new stack for example IDE’s, Repositories, tooling etc.

This trend seems intuitive considering that more information exists every day and we (humans) will not be getting better at understanding it anytime soon. 


