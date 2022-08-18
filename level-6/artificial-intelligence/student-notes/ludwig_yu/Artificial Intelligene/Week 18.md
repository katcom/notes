Week 18

# <section-title>Week 18</section-title>
**Learning objectives**
- Explain what a variational auto-encoder is, and give examples of applications for VAEs
- Describe the concept of a latent space and explain why they are important when exploring the capabilites of pre-trained models
- Load and use a pre-trained model to generate multi-track MIDI files

## <section-title> History of Automated Music Composition </section-title>
### Early Example
18th century: Musical Dice Games: selecting fragments of pre-composed music using dice

19th century: The Quadrille Melodist, Cards that 'generate' music pianists.

20th century: Schoenberg -> Ligeti, Xenakis, Stockhausen, Babbit 'Process Music'

1950s: Hiller's experiments with the llliac Suite

random selection
filtering by testing against rules
randomly generated markov chains

first example of writing program to generate music (in form of music scores)

#### The Music I language
"The reaction amongst all but a handful of people was a combination of skepticism, fear, generality and a complete lack of comprehsion"

Speical computer programming languages for creating sound synthesis patches. More about synthesis instead of composition

#### too many ideas?
"It's a change from the influences of scarcity or economy to the influences of abundance and waste" - Cage

1965 Koenig's PROJECT 1 composing program worked with tables of options covering chords, rhythm etc.

"The trouble taken by the composer with series and their permutations has been in vain; in the end it is the statistical distribution that determines the composition" - Koenig 1971
1970s Spiegel interactive system
"The program I wrote for Patch work had all Bach's favorite motivic manipulations- retrograde, inversion, augmentation, diminution, transposition avilable on switches, knobs, pushbuttons" Spiegel
Xenakis
"With the aid of electronic computers the composer becomes a sort of pilot: he presses the buttons, introduces coordinates and supervises the controls of a cosmic vessel sailing in the space of sound" Xenakis 1971

Xenakis, I. (1971). Formalized Music: Thought and Mathematics in Composition. Indiana Unversity Press

1980s: More complex techniques

"A method for automatically composing a new musical work based upon a plurality of existing musical work segments using a programmed linear retrograde recombinant musical composition algorithm" David Cope 2006

Taking in a number of music (for instances, all works by Mozart), and chopping them into pieces and then creating permutations of those

1980s Expert Systems
"The program takes input an alphanumeric encoding of the chorale melody, and outputs the harmonization in conventional music notation, and the hierarchical voice leading  analysis in slur-and-notehead notation" - Ebcioglu 1988

Ebcioglu, K. (1988). An expert system for harmonizing four-part chorales. Computer Music Journal 

1990s: A-life systems, L-systems, genetic algorithms
"In this paper, we adapt string re-writing grammars based on L-System"

GenJam : a jazz improvising system using a genetic algorithm. It plays solos over the accompaniment of a standard rhythm section. A human mentor gives real time feedback which is used to derive fitness values for the individual measures and phrases(the human is the fitness function)

2000s Machine Listening

2000s Popular Electronic Music

Collins was working on break beats and trying to re-create the sort of intricate chopped break beat patterns that you'd see an artist like Aphex twin square pressure. In fact, he built a square pressure simulator which is able to chop up break beats in a statistically similar pattern to two square pressure

2010s deep learning
OpenAI Jukebox, a model that generates music with singing in the raw audio domain


 ### subtitle
### subtitle
## <section-title> Latent Space </section-title>
### subtitle
### subtitle
### subtitle
## <section-title> title 3 </section-title>
### subtitle
### subtitle
### subtitle

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
	reading-section{
		display:flex;
		flex-direction:column;
		font-size:16px;
		font-style:italic;
		font-family:times;
	}
	reading-section-title{
		display:flex;
		text-align:center;
		justify-content: center;
		font-size:18px;
		font-style:italic;
		font-family:times
	}
	reading-section a{
		margin-top:10px
	}
	a{
		color:black
	}
</style>