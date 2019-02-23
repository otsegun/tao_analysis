---
title: "Tao Analysis Solutions"
author: "Oluwasegun Ojo"
date: "21 de febrero de 2019"
output: 
  html_document: 
    keep_md: yes
---



## My attempts at solving Tao Analysis I problems.

## Chapter 2 

### Prove that the sum of two natural numbers is again a natural number? (Pg 24)
Using induction on $n$, we have the base case to be:
$$0 + m := m$$
which is a natural number as desired (by definition of addition and **Axiom 2.1**). 
Now we assume that if $n$ and $m$ are natural numbers, then $n+m$ is also a natural number. We have to show that $(n++)+m$ is also a natural number. But 
$$(n++) + m = (n+m)++$$
by definition of addition and **Axiom 2.2**. However, $n+m$ is a natural number according to the inductive hypothesis and therefore $(n+m)++$ is also a natural number by **Axiom 2.2**.

### Prove that $n++ = n+1$ (Pg 26)
#### Solution 1
Since $n$ is a natural number, we have that $$n++ = (n++) + 0$$ according to **Lemma 2.2.2**. But this also gives $$(n++) + 0 = (n+0)++$$ according to definition addition. However, this further gives
$$(n+0)++ = n + (0++) = n+1$$
by **Lemma 2.2.3** and definition of increment respectively. QED

#### Solution 2
Using induction on $n$, we have to show that $0++ = 0+1$. However, we know that $$0++ = 1 = 0 + 1$$ by definitions of increment, and addition respectively. Now we assume that $n++ = n+1$, we have to show that $$(n++) ++ = (n++) +1$$
From the RHS, we know that
$$(n++)+1 = (n+1)++ = (n++)++$$
by definition of addition and the inductive hypothesis repectively. QED.

### Exercise 2.2.1 (Pg 26)

Prove that for any natural numbers $a$, $b$, $c$, we have $(a + b) + c = a + (b + c)$.

Using induction on $a$. For the base case, we want to show that $(0+b) + c = 0+(b+c)$. However, 
$$0+(b+c) = b+c$$ 
since the addition of two natural numbers is also a natural number and also by the definition of addition.
Next we assume that $(a+b)+c = a+(b+c)$, we have to show that $$((a++)+b)+c = (a++) + (b+c)$$  
From the RHS, we have that
$$(a++) + (b+c) = (a+(b+c))++ = ((a+b)+c)++$$
by the definition of addition and the inductive hypothesis respectively. Furthermore, 

$$((a+b)+c)++ = (((a+b)++)+c) = ((a++)+b)+c$$
by definition of addition. QED
### Exercise 2.2.2.

### Exercise 2.2.3.

### Exercise 2.2.4.

### Exercise 2.2.5.

### Exercise 2.2.6.
