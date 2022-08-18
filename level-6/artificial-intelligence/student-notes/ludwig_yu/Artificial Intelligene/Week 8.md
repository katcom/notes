Week 8

# <section-title>Week 8</section-title>

## Representing knowledge in logic
Knowledge can be encoded in many ways. But by encoding knowledge in logic, we can enable logical inference over knowledge.

Example:
Consider the statement
‘If an academic query was handled by the module leader, then it washandled correctly’

Representing and encoding the statement in logic enables a logical inference engine to determine if the statement is true or false.

### Logical Operations
$\neg A$ not A
$A \land B$ conjunction, A And B
$A \lor B$ disjunction, A OR A
$A \Rightarrow B$ implication, If A then B
$=$ equivalence, A if and only if B

## RDF
If something is defined in RDF, then it is defined globally and unqiuely

## Prolog
Prolog is good for solving problemsthat involve objects and relations between them.

The fact 'Pete raises a query_001' can be encoded as
`raises(pete,query_001)`

### Prolog terminology
- clauses is logical statements
- pete is an instance (starts with lower-case letter)
- Student is a variable (starts with Captial letter)
- raises is a relation or a predicate (starts with lower-case letter)

### Prolog inference
Input statement:
`raises(pete,query_001)`
Question:
`?-raises(pete,query_001)`
`?-raises(pete,x)`

The resopnse from Prolog after entering these statements
`?-raises(pete,query_001)
true`
`?-raises(pete,x)
query_001`

The attractive feature of the knowledge model is that it can be extended and integrated with other knowledge model

## Description Logic vs First-order Logic
The syntax of 
FOL is designed to say things about objects
DL is designed to define and describe objects

The inferences in DL are:
subsumption: if one class is subclass of another class
classification: checking to what class an object belongs

## Reasoning

## Deduction and Abduction
### Deduction:
pattern
If P, then Q         - condition
Q                        - assertion
Therefore, Q      - conclusion

Example:
Rule: All swans are white
Fact: Daffy is a swan
$\implies$ Daffy is white

subsumption
classification
prolog reasoning to identify the truth value of logical statement

### Abduction
Abduction, the pattern:
If P, then Q.       - condition
Q.                      - observation
Therefore, P      - possible explanation

Example:
Rule: All swans are white
Fact: Daffy is a white
$\implies$ Daffy is a swan (it could be wrong)

Generation of hypotheses by the Robot Scientist AI system
### Induction
Generalisation of facts
It is not guaranteed to be correct - a verification step is required
ML is based on inductive reasoning

Rule: Daffy is aswanand white
Fact: Tweety is a swan is a white
$\implies$ All swans are white 

## Hypotheses generation: abduction
- The robot scientist adam use abduction to generate hypotheses about gene functions
- background knowledge is a yeast metabolic pahtway model- a graph representing chemical reactions
- The metabolic graph is encoded in prolog, in FOL
-  Yest has about 6000 genes and their functions are similar to those in humans
-  It is still unknown what  genes are responsible for some of the reactions
-  It is possible that several genes are responsible for one reaction and one gene may be responsible for several reactions

Our knowledge may be not correct. Therefore the conclusion from abduction may also be wrong. Therefore, It needs experiements to verify our knowledge and update it when needed.

## Induction for hypotheses generation
Rule: Daffy is aswanand white
Fact: Tweety is a swan is a white
$\implies$ All swans are white 


- Generalisation of facts
- Not guaranteed to be correct
- Verification is required

ML
- ML is based on inductive reasoning
- Patterns in data are detected and generalised to new data
- Prediction is not necessarily correct.

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