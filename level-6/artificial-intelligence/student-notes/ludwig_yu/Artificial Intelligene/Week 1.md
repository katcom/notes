Week 1

# <section-title>Week 1</section-title>

Learning Objectives

- Explain the key features of a **genetic algorithm** and how they can be used to address a given problem
    
- Compare and contrast examples of **artificial life systems**
    
- Develop an argument about the potential of **evolutionary computing**
    

## Bioinspired Computing

Is Bioinspired Computing AI?
Yes

> “Bio-inspired computation has emerged as one
> of the most studied branches of Artificial
> Intelligence during the last decades

### Cybernetics

**Cybernetics** is the science of control and communication, in the animal and the machine, according to Weiner.

**Reading**:
Pickering, Andrew. "Cybernetics and the mangle:
Ashby, Beer and Pask." Social studies of science
32.3 (2002): 413-437. [link](https://www.researchgate.net/publication/2829265_Cybernetics_And_The_Mangle_Ashby_Beer_And_Pask)


> #### ABSTRACT
>   This paper aims to enrich our understanding of the history and substance of cybernetics. It reviews the work of three British cyberneticians - W. Ross Ashby, Stafford Beer and Gordon Pask - paying attention particularly to the materiality of their practice - the strange and fascinating devices and systems that were at the heart of their work - and to the worldly projects they pursued - scientific, technological, artistic, organizational, political and spiritual. Connections are drawn between cybernetics and recent theoretical work in science and technology studies, in the hope of illuminating key features of both. The paper concludes by suggesting that the antidisciplinary impulse of contemporary science studies might find inspiration in the work of cyberneticians - that theory does not have to remain confined to the realm of theory.


**Connectionism** (aka neutral networks)

The perceptron is a minimally constrained "nerve net" consisting of logically simplified neural elements, which has been shown to be capable of learning to discriminate and recognize perceptual patterns.

**Reading**
F. Rosenblatt, "Perceptron Simulation Experiments,"
in Proceedings of the IRE, vol. 48, no. 3, pp. 301-309,
March 1960, doi: 10.1109/JRPROC.1960.287598 [link](https://ieeexplore.ieee.org/document/4066017)

>Abstract:
An experimental simulation program, which has been in progress at the Cornell Aeronautical Laboratory since 1957, is described. This program uses the IBM 704 computer to simulate perceptual learning, recognition, and spontaneous classification of visual stimuli in the perceptron, a theoretical brain model which has been described elsewhere. The paper includes a brief review of the organization of simple perceptrons, and theoretically predicted performance curves are compared with those obtained from the simulation programs, in several types of experiments, designed to study "forced" and "spontaneous" learning of pattern discriminations.

### Artifical Life

"Life as it could be" 
What kind of life is possible in the simulated system

**Reading**
D. B. Fogel, "Nils Barricelli - artificial life, coevolution, self-adaptation," in IEEE Computational Intelligence Magazine, vol. 1, no. 1, pp. 41-45, Feb. 2006, doi: 10.1109/MCI.2006.1597062 [link](https://ieeexplore.ieee.org/document/1597062)

> Abstract:
Nils Aall Barricelli was one of the pioneers in evolutionary computation. His publication of "Esempi Numerici di processi di evoluzione", a study in what would now be called artificial life, in the journal Methodos, in 1954 is perhaps the earliest published record of an evolutionary simulation. The paper was republished in 1957 in English, and detailed the results of programs that were run at the Institute for Advanced Study in Princeton, NJ, in 1953.
>Barricelli’s  initial  experiments  comprised a simple simulation of numbers in a grid. The numbers moved in the grid according to local rules that were specified  for  each  number.  For  example, suppose that a one-dimensional grid had N = 20 cells and numbers were distributed  in  those  cells  at  the  initial  generation  g = 0.  For  g = 1,  the  numbers would  shift  to  different  cells  based  on the  arrangement  of  numbers  at  g = 0 and  then  progress  further  or “migrate”based on their then-current positions. 


Neumann, János, and Arthur W. Burks. Theory of self-reproducing automata. Vol. 1102024. Urbana: University of Illinois press, 1966 [link](https://cba.mit.edu/events/03.11.ASE/docs/VonNeumann.pdf)

## Evolution Theory
1. Population
Population has **variations**. A type of creatures, aka species, has different versions of it.
Population also has **heredity**. The variation is inheritable. That is, if the creature are to reproduce, its offsprings would look like them, but there are also slight variations, espically when it comes to crossbreeding.

2. Selection
Creatures fight for survival, such as overcoming difficulties to get foods they need. The strong one that has features allowing it to overcome the difficulties would have its reward (such as foods). The weak one that has features stopping it from overcoming the challenges would lose the rewards.
3. Breeding
 The successful one can reproduce. There would be more of them.
 
**Reading:**
Clegg, Kester. "An Introduction to Evolution for Computer Scientists." (2008).[link](https://www-users.york.ac.uk/~gt3/Lectures/images/YCS-2008-425.pdf)
* * *
### Genotype vs. Phenotype
Important concepts:

 **Nature** defines what an individual could do. What it starts with in life.

**Nurture** is the process that the individual goes through its life.
#### Genotype
The genotype encodes the range of characteristics of the individual. 

**DNA** is nature.  DNA is passed from one generation to the next(heredity). 

Environment is **Nurture**. Whether it has easy access to foods nearby, for example.

#### Phenotype

The phenotype is the actual individual that develop s in the world, as the result of the nurture.

For example, if two animal with the same DNA (genotype) are born to the world, but one in the place that has more food while the other in the place with less foods, they would develop differently and have different phenotype.

DNA is a four-letter sequence AGTC. These are the alphabet of DNA.

DNA in a cell would consists of a sequence of these four letters. DNA would then develop into proteins. 

Three letters forms a group that is mapped to a set of amino acid. A string of amino acid folded into a 3D structures which constructs a protein.

For example, suppose this is a string of DNA
> AAGTCAGGTCCA

Here is a mapping of this sequence to amino acid. The number represents the type of the amino acid that the three-letter DNA fragment is mapped to. 

> AAG TCA GGT CCA
> 1       3      5       8

These new sequence of amino acid (1-3-5-8) would then fold into a complicated 3d structure.  This 3D structure is the phenotype.

The environment applies selective pressure to the phenotypes. The **fit** phenotypes are more likely to survive to reproduce, while the underlying genotype provide heredity.
* * *
## Genetic Algorithms

Genetic algorithm is a probabilistic search procedures designed to work on large spaces involving states that can be represented by strings. In other words, genetic algorithm is a search algorithm that searches in a large spaces of states, which are represented by strings (such as 'AAG TCA GGT CCA')

With respect to Evolution Theory, the **probabilistic search** is the **Selection**. 
The **states** is the **phenotype**. 
The **strings** are **genotype**.

The *space* is defined as the space of possible solutions to a problem. Searching the space is equal to finding the solution to a problem

**Examples of problems:** 
What is the ideal shape for an aeroplane wing? 
What are the ideal settings for this data centre to reduce power 
consumption?

#### How genetic algorithm works?
#### Selection:
Test the individual, and give them a fitness score according to the fitness function.
**Rulette wheel selection**: population are presented as a portion in the pie chart. We spin the wheel to choose which two individuals are to reproduce. The size(chance of being selected) of the their part depends on their fitness score. The higher the score, the greater the portion, hence the greater chance to be selected to breed.
#### Crossover breeding:
Select some bits from the first parent and some bits from the second parent.
#### Mutation:
Mutate the child slightly. Pick random bits in the DNA string and flip them to generate mutation. Multiple rounds of mutation could be used.
#### Start Again
Go back to do the selection, wheel, crossover breeding and mutation
**Reading**:
Holland JH. Adaptation in natural and artificial 
systems: An introductory analysis with 
applications to biology, control, and artificial 
intelligence. University of Michigan Press 1975

Goldberg, David E., and John H. Holland. 
"Genetic Algorithms and Machine Learning." 
Machine Learning 3.2-3 (1988): 95-99
[link](https://www.semanticscholar.org/paper/Genetic-Algorithms-and-Machine-Learning-Goldberg-Holland/c61134ada9f0e3f3373d635c31a8b3caa37f9977)
* * *
### Why Genetic Algorithm Works
“The question that most people who are new to 
the field of genetic algorithms ask at this point 
is why such a process should do anything 
useful”

There are local maxima and global maxima in the search space. Genetic Algorithms allow us to bypass the local maximums and to find the global maximum. There are three ways to accomplish this according to John Hollan

#### Hyperplane Sampling
We freeze some bits and allow other bits to change. The focus of the the hyperplane sampling is the genotype. We can consider this bit of genotype is good, and we don't change it. Rather, we change other bits and see what will happen.
#### Implicit Paralleism
Maintain multiple "blood lines" within the population. We do not only optimize one solution, but also optimise multiplie possible solutions. We can even recombine those solutions at the same time. (roulette wheel) 

#### Computational Parallelism
We can assess different solutions at the same time on the multi-processor systems. It is more about programming rather than modeling the selecation process of the population.
**Reading:**
Whitley, Darrell. "A genetic algorithm tutorial." 
Statistics and computing 4.2 (1994): 65-85 [link](https://www.researchgate.net/publication/2425017_A_Genetic_Algorithm_Tutorial)
>This tutorial covers the canonical genetic algorithm as well as more experimental forms of genetic algorithms, including parallel island models and parallel cellular genetic algorithms. The tutorial also illustrates genetic search by hyperplane sampling. The theoretical foundations of genetic algorithms are reviewed, include the schema theorem as well as recently developed exact models of the canonical genetic algorithm.
>
* * *
### Morphology And Sim's Creatures
#### What is Morphology
> "the scientific study of the structure and form of 
animals and plants"

by Cambridge English Dictionary

Sims paper describese a novel system for creating virtual creatures that **move** and **behave** in simulated 3d physical worlds.
* * *
### Sim's Creatures:
#### Biomorph
A graph representation of the organism generated in the computer, used in Evolution model
#### Morphology:
Morphology is represented in an abstract graphing system to assist the programming of the creatures system.

#### Simulating Creatures
“Dynamics simulation is used to calculate the 
movement of creatures resulting from their 
interaction with a virtual three-dimensional world.”
Sims ran the creature in simulation in CM5 a fastest computer in the world 1993

#### Control system:
Mapping from **sensor input** to **actuator output**.
Lots of neurone type.
**Sensor inputs** help the creature recognise what is going on in their surroundings.

**Motor outputs** help the creatures move within the world(it is best to move in response to what they sense)
#### The fitness function
“In this work, virtual creatures are evolved by 
optimizing for a specific task or behavior.”

Various fitness function, competing task.
For example, a **walking fitness function** could be used to measure how far the creatures could walk. This fitness meaure produced a number of simple creatures that can walk in a fairly fast speed in Sims paper.

#### The Next Generation
“Offspring are generated from the surviving 
creatures by copying and combining their directed 
graph genotypes. When these graphs are reproduced 
they are subjected to probabilistic variation or 
mutation, so the corresponding phenotypes are 
similar to their parents but have been altered or 
adjusted in random ways.” 

Next generation is created from the creatures surviving from the given task, copying and combining their directed graph henotypes. When these graphs are reproduced, some probabilistic variation and mutation are applied. 
For example: increase the amount recursion on some nodes, increasing the number of connections between on another or add a new connections.
#### Result:
“The walking fitness measure also produced a 
surprising number of simple creatures that could 
shuffle or hobble along at fairly high speeds. Some 
walk with lizard-like gaits using the corners of their 
parts. Some simply wag an appendage in the air to 
rock back and forth in just the right manner to move 
forward."

The walking fitness measure also produced a surprising number of simple creatures that could shuffle or hobble along at fairly high speeds.

#### The significance of Dawkin's work on Biomorphs:

It shows that even simple genetic algorithm can generate highly complicated creatures. Therefore it proves that the evolution theory can give arise of highly complicated creatures in the world without intellengent design

Using small mutations of biomorphs - abstract figures made to look vaguely like creatures in nature, Dawkins clearly showed how the process of evolution can create very complicated organisms if given a long period of time. 

It is presented as a counter-argument to the idea of `intelligent design` - where the complexity of life is said to attest to the existence of a higher creator-being, commonly denoted as `God`.

**Reading:**
Sims, Karl. "Evolving virtual creatures." 
Proceedings of the 21st annual 
conference on Computer graphics and 
interactive techniques. 1994 [link](https://www.cc.gatech.edu/~turk/bio_sim/articles/sims_virtual_creatures.pdf)

> Abstract
> This paper describes a novel system for creating virtual creatures
that move and behave in simulated three-dimensional physical
worlds. The morphologies of creatures and the neural systems for
controlling their muscle forces are both generated automatically
using genetic algorithms. Different fitness evaluation functions are
used to direct simulated evolutions towards specific behaviors
such as swimming, walking, jumping, and following.
A genetic language is presented that uses nodes and connections as its primitive elements to represent directed graphs, which
are used to describe both the morphology and the neural circuitry
of these creatures. This genetic language defines a hyperspace containing an indefinite number of possible creatures with behaviors,
and when it is searched using optimization techniques, a variety of
successful and interesting locomotion strategies emerge, some of
which would be difficult to invent or build by design.


<style>
section-title{
    color:black;
	text-align:center;
	display: flex;
    justify-content: center;
	background:white;
}
section-content {
	display:flex;
    text-indent:1em;
}
p {
    text-indent:1em;
}
</style>