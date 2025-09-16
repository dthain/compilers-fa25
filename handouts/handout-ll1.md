**CSE 40243 - Week 4 Handout - LL(1) Grammars**

Consider the following grammar:
```
P -> S $
S -> repeat S ;
S -> print E ;
S -> L = E ;
E -> E @ E
E -> E # E
E -> ^ E
E -> ( E )
E -> L
L -> id
L -> id[E]
```

1 - Rewrite the grammar into LL(1) form.

2 - Compute the FIRST and FOLLOW sets for your rewritten grammar.

