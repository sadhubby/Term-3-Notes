#csintsy
Intelligent Systems
	- Computation systems that perceive, evaluate and decide their actions in ways that a human would.
	- Are used to **assist** humans.

Artificial Intelligence
	- Backbone of intelligent systems
	- study of how machine can exhibit at least one aspect associated with intelligent behavior, such as:
		1. Problem Solving: performance of non-trivial goal-directed tasks
		2. Reasoning: drawing logical inferences from facts
		3. Learning: improvement of performance through experience

### **Modelling Inference Learning Paradigm**

Real-world problem - > Model
	Modelling: representing a real world task into an abstract model
Model -> Answer / Solution
	Inference: answer questions / find solutions to the problem, algorithms
Model - > Fine-tuned model
	Learning: sometimes, models can be fine-tuned based on historical data
	
Example:
- Real world problem: find a route from one place to another in manila considering the traffic.
- Modelling: use a weighted graph to model the problem
	- Nodes: places / junctions
	- Edges: roads
	- Weights: amount of traffic on that road
- Learning: Improve the weights assigned to each edge based on historical data observed in the real world

3 Types of AI:
1. Symbolic AI: top-down approach
	 Identify the "rules" of the problem and model it
	 Find a solution based on rules
2. Neural AI: bottom-up approach
	 Start with examples then feed to model
	 Adjust the "rules" of the model based on the data
3. Statistical AI: view of mathematicians
	 provides mathematical rigor to AI approaches

Types of AI Models:
1. Reflex-Based Models: 
	- single-pass processing of input features to map it to an output
2. State-Based Models:
	- represent the problem as a set of states to search through.
3. Variable-Based Models:
	- represent the problem as a set of constraints to satisfy.
4. Logic-Based Models:
	- automatic deduction and reasoning based on known facts

# ----  Continuation of AI Overview ----

### The Turing Test
1950: Alan Turing made the Turing Test. 
	propose the Turing test as a philosophical framework for artificial intelligence
The Turing Test goes like this:
	a Human Evaluator (C) talks with a machine (A) and a human (B)
	C cannot see A or B and they must communicate by typewritten messages (text)
	A must convince C that A is NOT the machine

### Birth of AI as a Field
1956: John McCarthy organizes a workshop at Dartmouth College with this goal: 
> precisely describe every aspect of learning and intelligence so that a machine can be made to simulate it

Early successes of AI include:
	1952 - Samuel's Checkers
	1955: Newell and Simon's Logic Theorist
	1950s to 1960s: Machine Translation
	Prominent paradigm was symbolic AI

Machine Translation
	1950s to 1960s: a lot of hype around machine translation
	However, despite it...
- Rule based machine translation faced problems
- Cannot handle semantic ambiguity and other linguistic nuances
1966: the government published report, concluding machine translation was:
- slower
- less accurate
- twice as expensive
This resulted in significant cuts in funding, leading to first AI winter

### First AI Winter (1974 - 1980)
- a period of reduced funding and interest in artificial intelligence research
- The AI field is notorious for having hype cycles, followed by disappointment and criticism

### Knowledge-Based Systems
- 1970s-1980s: 
	- AI research heavily shifted to expert systems
		- Allows domain experts to encode their knowledge into system
		- Narrower focus (domain-specific)

### Notable Expert Systems
1. CADUCEUS - Medical diagnosis based on symptoms
2. MYCIN - Identifying bacteria that caused infections and recommending antibiotics
3. DENDRAL - analyzing and identifying chemical compounds
4. R1 / XCON - Assists users on selecting computer system components based on specs

Expert systems were able to have commercial and industrial impact

### Second AI Winter  (1987 - 2000)
- Problems with Expert Systems
	- cannot handle uncertainty in the real world
	- Difficult to maintain rules in knowledge base
1987: the LISP market  crashes because there were not enough killer apps and the second AI winter starts

### The Roots of Neural AI

1943: McCulloch and Pitts publishes the first mathematical model for an artificial neural network

1958L Rosenblatt publishes the Perceptron learning algorithm

### Resurgence of Neural Networks
1960s: Multi-layer perceptrons were introduced
1986: Popularization of the backpropagation learning algorithm
1989: Application of convolutional neural networks to recognize handwritten digits by Yann LeCun

### Deep Learning
To put it simply: neural network with many hidden layers

2012: AlexNet makes big progress in object recogniition
2016: AlphaGo defeats world Go champion Lee Sedol with deep reinforcement learning

### AI Today
- ubiquitous in our daily lives
- used to be purely academic endeavor, now integrated into mainstream