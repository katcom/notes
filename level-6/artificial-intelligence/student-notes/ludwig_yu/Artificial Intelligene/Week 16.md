Week 16

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
# Week 16

## <section-title>Case Study Overview</section-title>

### <section-title> Overall Aim</section-title>

We are going to create a system which can generate a complete piece of music including lyrics, melody and singing

### Week 1 Generative systems

<p>
Learning about generative systems
Building a simple text generator from scratch
</p>

### Week 2 Generating Lyrics

<p>
Learn about a state of the art text generator
learn about fine tuning. 

Use GPT-2 to generate lyrics
</p>

### Week 3 Generating Music with Google Magenta Music-VAE

<p>
Learn about latent spaces
Use tensorflow-js and magenta-vae to generate complete musical arrangements
</p>

### Week 4 Generating Singing

<p>Learn about the challenges of voice, and especially, singing synthesis

Use a deep network based singing voice synthesizer to generate tuned singing from a list of notes and a set of lyrics</p>

### Week 5 Putting it all together
<p>
Select a chord progression
Mixing the music with singing
Rendering out the complete product
</p>

## <section-title> Generative System</section-title>

MYK defines two kind of tools:

- Active Tools
- Passive Tools

### Active Tools
<p>
The tools that can automatically finish the artwork. It actively process what the artist is doing and tries to interpret it and adding things to it. </p>

### Passive Tools
<p>
Everything is a result of the artist doing things on the art piece. If the artist stops, then nothing happens.
</p>

### Taxonomy
<p>
Boden and Edmonds 11 definitions, examples:
2\. C-art (computer art, such as drawing with digital tools) uses computers as part of the art-making process.
5\. G-art (generative art), at least in part, by some process that is not under the artist's direct control
6\. CG-art is produced by leaving a computer program to run by itself, with minimal or zero interference(interaction? problematic defintion) from a human being

- Features
- System Architecture
- \# of Agents
- Roles of human
- Environment
- Corpus
- Input
- Output
- Communication
- Human interactive modality
- Task
- Evaluation

It is not easy to evaluate which system is better in terms of computer generative artwork
</p>

## <section-title> Markov Model </section-title> 
<p>
The Markov model starts with a word sequence:
"The problem with the pop music industry is the music"

We can convert that into a first order model by making a state transition table.
</p>

### First order model

<p>
first order: the state only describes one word.
The first word "The" is the first state, which is followed by the second state "problem" .. etc.

In this manner, we would end up with this basic transition table:


<center>

|  State   |  Possible Next States    |
| --- | --- |
| The   |  problem, music, pop   |
|Problem| with|
|With|the|
|Pop|music|
|Music|industry|
|Industry| is|
|Is| the|

</center>

</p>

### Generative process
<p>

1.  pick a random state from observed states
2.  Select from the possible next states
3.  If no possible next state, back to 1
</p>

### Second Order
<p>
Second Order: consider the two previous states.
</p>

### How are more complex models different
<p>
They have a more complex model of the sequence than a transition table.

They have a more complex method for picking the next state/output, including more complex state.
</p>

### Example of more complex generative text models
<p>

1. Variable order markov model
2. Long short term memory network
3. Transofrmer network
</p>

