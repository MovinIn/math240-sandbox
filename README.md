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
