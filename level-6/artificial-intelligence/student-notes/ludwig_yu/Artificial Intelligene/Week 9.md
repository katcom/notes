Week 9

# <section-title>Week 9</section-title>

Learning Outcomes

- Compare and contrast classical and real-world planning problems
- Explain the key steps for planning of experiments by Robot Scientist
- Explain how the Robot Scientists analyse experimental result

## Classical Planning

Classical planning deals with observable deterministic situtation. Given an initial state, a list of possible actions and their results, find a sequence of action that leads to the goal state.

## Planning in the real world

- In partially observable, non-deterministic, or unknown environment.
- Open-word instead of closed-world assumption
- Contingent planning
- Monitoring and re-planning

If something is not defined in the knowledge based, it is unknown. By contrast, in the classical planning, if something is undefined in the knowledge base, it means that thing does not exist.

### Scheduling

In real world,
Planning focuses onwhat to do and in what order
Scheduling adding constraints -- time and resources
"plan first, schedule later approach"

### Multi-agent planning

- An extra layer of planning and scheduling may require for multi-agent environments to coordinate agent's actions
- Generating plans for joint actions - joint planning
- Agents may share the same goal and the same representations
- The agents may cooperate in achieving the same goal
- Communications between agents may be required.

## Testable hypotheses

- Not all formulated hypotheses can be tested
- Some hypotheses may be tested in one laboratory but not in the other. That depends on the available equipments
- If a hypothesis can't be tested, then instead a related hypothesis can be tested.

Knowledge for plannning experiments
The planning agent needs to know available equipments and their functionalities.
We developed LABORS to assist in experiment planning

## Aanalysing Experimental Results


Machine Learning
- Robot Scientist used decision trees to decide if the growth of yeast strins was affected by the addition of specified metabolites or not
- The difference between the growth of a wild type and a mutant can be subtle
- Experiments were replicated
- This enabled the detection of subtle diffrerences in a statistically significant manner
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