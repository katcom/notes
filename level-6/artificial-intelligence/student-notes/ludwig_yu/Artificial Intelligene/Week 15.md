Week 15

# <section-title>Week 15</section-title>

**Learning Objectives**
- Present examples of human-competitive AI game players
- Reason about the impact of human-competitive AI game players on human beings
- Justify the trend towards general AI and discuss its potential impact on society

## <section-title>State of the Art AI Game Player  </section-title>
### After DQN
Double DQN
DreamerV2 (great reference set)
R2D2
Agent57

Answer these questions:
- What does the agent do?
- How does it gather experiences
- How does it build that state transition matrix
- How does it gain understanding of how the environment operates(in DQN it is the replay buffer)
- Beyond epsilon and greedy, what is the exploratory behavior is required to get better performance?
- 
- NN Architecture?
- What kind of the NN architecture do these systems use
- What was the loss function
- How to compute the ground truth when you don't have a ground truth?

#### Double DQN- Rainbow
<p>
 What was the loss function?
 KL Loss

 What is the neural network architecture?
  Dueling network architecture
 </p>
### Star Craft - Alphastar
Alphastar uses various techniques
### Dota II - OpenAI 5

7215 wins, 42 losses
### Mario AI Competition
Ran 2009-2012
Turned into the platformer AI Competition

Check out the Ms. Pac-man competition

##  <section-title>Ethics of game playing AI </section-title>

### 6-dimensions of fairness
- **Perceptual** human and AI can both see the pixels of the game
- **Motoric** human needs time to make the action, however, AI is much faster
- **Historic** simulation can be speeded up in training, AI can play espsodes equalivent to 100 year, however, human can only play the game in normal speed
- **Knowledge** speical knowledge? similar to perceptual. In dota, human can only see a part of the map, whereas AI can see the whole map
- **Compute** do the two systems have the same computational power 
- **Common-sense** AI can do well in playing dota, but it cannot pour a couple of tea
### A More Moderate View
No fair competition between AIs and human has occurred in Dota 2 and StarCraft II

### Direct Impact of superhuman players on game players

The lessons that AlphaGo is teaching us are going to influence how Go is played for the next 1000 years - commentator in AlphaGo, the movie. This is good, positive

However, the south korean player said that he decided to retire after realising: "I'm not at the top even if I become the number one"

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