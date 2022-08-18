Week 11

# Week 11

2015 Generalised human level AI video game player

DeepMind's Deep Q Network agent

Part I: Some history and the breadth of the research field

Part II: Formalising how an AI can learn a game

Part III: Tooling - OpenAI gym, convolutional neural networks

Part IV: Expressing the formalism in code, Training and running an agent

Part V: State of the art and ethics in AI game players

**Learning Objectives**

- Explain how the DQN agent architecture and learning system is expressed as a working program
- Evaluate the performance of a DQN agent
- Deploy a pre-trained neural network and use it to play games in real-time

### What is game playing AI and what is not

AIs that play games. It is not a AI player that plays games against human

### Why play games with AI

> Games are interesting because they are too hard to solve
> 
> \- Russell, Stuart, and Peter Artificial Intelligence: a modern approach
> 
> Researchers have considered StarCraft to be the hardest game for computers to play, which ultimately suggests that this fame is the final grand challenge for AI in games before tackling real-world problems
> 
> \- When Are We Done with Games, Justesen, Debus

An interesting / brave paper lay some milestones for AI in 2018

They asked experts to estimate when AIs would meet human level in various tasks, including playing games

Reading list

1\. Grace,"When will AI exceed human performance? Evidence from AI experts"

2\. Badia, Puigdomenech "Agent57: Outperforming the atari human benchmark"

3\. Russell, Stuart, and Peter Artificial Intelligence: a modern approach

4\. When Are We Done with Games, Justesen, Debus

### Commercial interest

Computer-controlled characters / game elements have been there since the start.

Also it is helpful to playtesting.

> Relying exclusively on playtesting conducted by humans can be costly and inefficient. Artificial agents could perform much faster play sessions, allowing the exploration of much more of the game space in much shorter time.
> 
> \- Zhao et al. "Winning isn't everything: Training agents to playtest modern games"

Reading:

Zhao et al. "Winning isn't everything: Training agents to playtest modern games"

### Research Themes

### Moravec's paradox

Things that humans find hard, it is easy for AI

Things that humans find easy, it is hard for AI

This leads to the trend of generalization in game-playing AIs: AIs that can play multiple games

### General game players

Agent57 is state of the art in 2020

### When will it end?

> "An ultimate goal that would demonstrate that an AI system can fully master a game, beyond the extrinsic factors of human vs. human competitions, would be to allow anyone to play against it over a long period of time"
> 
> \- When Are We Done with Games, Justesen, Debus

## History of AI Players

1950 Shannon, Seminal work on chess playing algorithms

1952 Strachey, Checkers / drafts

1979 Berliner, Backgammon,

1992 Schaeffer, A world championship caliber checkers program

1997 Campbell, Deep Blue

2002 Sheppard, Scrabble

2007 Schaeffer, Checkers is solved

2012 Togelius, Julian, The mario AI championship

2015 Mnih, Human-Level control through deep reinforcement learning

2016 Silver, Mastering the game of go without human knowledge

2018 Brown,Noam, Tuomas, Superhuman AI for heads-up no limit poker: Libratus beats top professionals

2019 DOTA II, Raiman, "Long-term planning and situational awareness in OpenAI five"

2020 Badia, Agent57: Outperforming the atari human benchmark

The Computer Olympiad: Computer vs. computer

**How might we build a game playing AI?**

We build an AI using DQN agent that can learn to play Atari video games. The DQN agent uses reinforcement learning

Questions to solve:

- How do I get points
- which way is the ball going
- where are the bricks
- How can I get  the ball on the correct side

AI get the pixels of the screen

We tell AI the current score

AI outputs: left,right or nothing

**Solutions:**

We could make an input-output dataset:

1\. we can train a big network to learn the mapping, but it is very expensive.

2\. we can use reinforcement learning

**What is reinforcement learning?**

"How agents can learn what to do in the absence of labeled examples of what to do"

"Imagine playing a new game whose rules you don't know; after a hundred of so moves, your opponent announces," you lose.". This is reinforcement learning in a nutshell"

Russel，"Artificial intelligence: a modern approach,p830-831"

Thinking about Reinforcement learning

States, Actions, Rewards