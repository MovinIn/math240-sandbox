# math240-fall
## logistics
attendance not taken (lectures)  
exams are not cumulative  
80% of zybook participation activities => 100% credit  
2 discussion section drops  

## overview
discrete structures - can be enumerated!  
## logic & proofs
`induction`
1. shows some property holds for all items in a discrete structure
2. used to show program correctness

`recursion`:   
`program analysis`: big O, big theta, etc. (time complexity!)
### Axioms
An `axiom` is a statement that is preconceived to be true.   
### Propositions
A `proposition` is a statement that can be either true or false, but not both.   
$$P \implies Q$$ is `false` if $$P$$ is true, but $$Q$$ is false. Otherwise, $$P \implies Q$$ is `true`.   
$$P \iff Q$$ means $$P$$ is `T/F` if and only if $$Q$$ is `T/F` respectively. This statement is also logically equivalent to $$(P \implies Q) \land (Q \implies P)$$  
$$P \land Q$$ is true if and only if $$P$$ is true AND $$Q$$ is true.   
$$P \lor Q$$ is true if $$P$$ OR $$Q$$ is true.   
#### Order of operations
<img width="131" height="105" alt="image" src="https://github.com/user-attachments/assets/b3264b7c-5ef2-4da2-b403-6b9d7a242055" />

#### Identities
<img width="1057" height="668" alt="image" src="https://github.com/user-attachments/assets/1bf93b62-e83a-47ad-8ece-a756ddfc448b" />  

## Division Algorithm
Let $$x \neq 0$$ and $$y$$ be integers. $$x | y$$ means that there exists an integer $$k$$ such that $$y=kx$$.   
If $$x | y$$ and $$x | z$$, then $$x | (ky+jz)$$ for any integer $$k$$ and $$j$$.   
$$x \text{ div } y = \text{floor}(x/y)$$  `// the floored quotient.`  
Let $$q = x \text{ div } y$$. $$x \text{ mod } y = r$$ such that $$y = qx+r$$, $$0 \le r \ge x-1$$.  
## Prime factorization
`relatively prime`: two integers $$x$$ and $$y$$ are relatively prime if the greatest common factor between them is 1.   
<img width="1083" height="421" alt="image" src="https://github.com/user-attachments/assets/6e6f264b-f752-4a9c-a574-cb110cd491c0" />  
## floor/ceil
<img width="736" height="47" alt="image" src="https://github.com/user-attachments/assets/4303bd45-b2a1-451a-806a-5b4a36f25ac1" />
<img width="808" height="42" alt="image" src="https://github.com/user-attachments/assets/42549ae5-8881-432a-9de5-2a510de3a44d" />

## Sets
$$A \cup B \iff \\{ x: x \in A \lor x \in B \\}$$  
$$ A \cap B \iff \\{x: x \in A \land x \in B \\}$$  
$$ A \oplus B \iff \\{x: (x \in A \land x \notin B) \lor (x \in B \land x \notin A) $$  

<img width="442" height="44" alt="image" src="https://github.com/user-attachments/assets/fc2e1459-e7cf-4d86-bca4-145e54061fdc" />  

If $$A$$ and $$B$$ are finite sets, then: <img width="205" height="37" alt="image" src="https://github.com/user-attachments/assets/0277e2c5-89c9-496b-ad61-3924e7289cd5" />  

$$A^k$$ is $$A \times A \times A ... \times A$$ $$k$$ times.   
$$\lambda$$ represents the empty string of length 0.  
Let $$s$$ and $$t$$ be strings. $$st$$ is $$s$$ and $$t$$ concatenated together. 

<img width="411" height="109" alt="image" src="https://github.com/user-attachments/assets/122f8770-d4ac-4865-b5a6-6eac44b321d2" />  
<br/>
<img width="155" height="66" alt="image" src="https://github.com/user-attachments/assets/ebcab929-b716-467f-90fe-fb6651c5f02f" />  

### Set Identities
<img width="975" height="645" alt="image" src="https://github.com/user-attachments/assets/9e36253b-97b8-4b81-9beb-2e0b878da116" />  

Let $$A = \\{3, 4, \\{1, 2\\}\\}$$. $$\\{1, 2\\} \notin A$$. $$\\{\\{1, 2\\}\\} \in A$$.

### Countable Sets
A `countable set` is countable if each of its members can be mapped to a one-to-one enumeration of the natural numbers.   
For example, finite sets are countable. The set of all integers is countable. The set of all rational numbers is countable.   
However, the set of decimal expansions are not countable. For example, the decimal 0.5 cannot be mapped to an index (there are infinite numbers between the decimals 0.0 and 1.0).  
`closed under multiplication/closure`: $$\forall (x,y \in Z) (x*y \in Z)$$
### Uncountable Sets
An `uncountable set` is uncountable iff it is NOT countable.
## Proofs
Justification vs. Proof - Justification is often handwavey, proofs are often more formal.   
Often proofs are done with cases (ie. $$k>0$$, $$k<0$$, $$k=0$$).  
#### Proof by Contradiction
1. Start with Proposition
2. Apply Transformations that preserve Truth Value
3. Eventually reach a tautology or a contradiction
#### Direct Proof
1. Start with a Proposition
2. Assume that it is True
3. Apply logical steps
4. Reach a tautology or reach (a=a).
#### Proof of Propositions
1. Start with Axioms
2. Apply transforms until we get to desired proposition.
### Logical Reasoning
An `argument` is a sequence of propositions, called `hypotheses`, followed by a final proposition, called the `conclusion`.   
An argument is `valid` if the conclusion is true for every truth assignment that makes every hypothesis true; otherwise, the argument is `invalid`.   
Let $$h_1$$, $$h_2$$, $$h_n$$ be hypotheses of an argument, and $$c$$ be the conclusion. The argument is valid if $$h_1 \land h_2 \land ... \land h_n \rightarrow c$$ is a tautology. 
### Rules of Inference

<img width="336" height="837" alt="image" src="https://github.com/user-attachments/assets/a0026499-33ec-49b6-b927-2288dada19cd" />

Example:   
<img width="934" height="600" alt="image" src="https://github.com/user-attachments/assets/5677d9f6-2538-47b4-9f60-b633a20b4cf5" />  

### Mathamatical definitions
`parity`: if two numbers are both even or odd, then the numbers have the same parity. Otherwise, the two numbers have opposite parity.  
`rational #`: $$r$$ is rational if there exists two numbers $$x$$ and $$y$$ such that $$r=\frac{x}{y}$$.
`prime #`: $$p$$ is prime iff $$p>1$$ and the factors of $$p$$ are $$p$$ and $$1$$.   
`composite #`: $$c$$ is composite iff $$c>1$$ and there exists an integer $$m$$ such that $$1<m<n$$ and $$m$$ divides $$n$$.   

## Sequences

Geometric

<img width="851" height="216" alt="image" src="https://github.com/user-attachments/assets/effbea3b-1684-4c99-8095-e838072a04f1" />  

Arithmetic

<img width="857" height="236" alt="image" src="https://github.com/user-attachments/assets/95948f9f-a145-4bba-a0a2-c94354d8ca69" />

## Induction
### Standard Induction 
We use induction to prove some predicate $$P(n)$$ for all $$n \ge h$$.
1. Prove base case $$P(h)$$.
2. Assume $$P(k)$$ holds for all $$k \ge h$$ `(Inductive Hypothesis)`
3. Prove for $$P(k+1)$$ using `(IH)`
### Strong Induction
We use strong induction to prove that if $$P(x)$$ holds for some $$x \le k$$, it implies $$P(k+1)$$  
We use strong induction to prove some predicate $$P(n)$$ holds for all $$n \ge k$$.   
$$P(x)$$ holds for all $$0 \le x \ge h$$ proves $$P(k+1)$$. 
1. Prove base cases $$P(0), P(1), \ldots , P(k)$$.
2. Assume $$(P(0) \land P(1) \land P(2) \ldots \land P(k))$$ holds for every $$k \ge 1$$.
3. Prove $$(P(0) \land P(1) \land P(2) \ldots \land P(k)) \implies P(k+1)$$ `(Inductive Hypothesis)`
## Algorithms

