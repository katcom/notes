Week 2

# <section-title>Week 2</section-title>

## GA
- GA starts with varied population with heredity
- test the individuals
- variations of the survivors

> “The most creative and challenging parts of programming a GA are usually the problem-specific aspects”

#### Reading:
<i>Harvey, Inman. "The microbial genetic algorithm." European conference on artificial life. Springer, Berlin, Heidelberg, 2009</i>


Phenotype: similar to Sims, but simplified

### URDF format
XML files
Unified Robot Description Format

An XML based file format for specifying robot 
models, including their motors and other 
dynamics

Why we use URDF?
- Programmatically generating models is difficult.
- We can share models

Links = nodes
Joint = edges
Joint can have angles, movability
nanonan
**Toturial**: [link](http://wiki.ros.org/urdf/Tutorials/Building%20a%20Visual%20Robot%20Model%20with%20URDF%20from%20ScratchA)
### Simulation
We use pybullet as physis engine
### Genotype
Similar to Sims,directed graph
### Fitness function
How far does it move?
But they are going to cheat, we need to find a way to stop the GAs from cheating
### Compute in parallel
we can gain speed up by setting things in parallel

### Technology Stack
Python
Pybullet as the physics engine
URDF format as genotype

#### Soft body physics
things can be deformed

## Joints and Movements
Different types of Joints
JOINT_REVOLUTE: can rotate
JOINT_PRISMATIC: can move along an axis
JOINT_FIXED: cannot move

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