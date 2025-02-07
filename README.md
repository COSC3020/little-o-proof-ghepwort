# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

## Answers

By definition, $o(g(n))$ means $f(n)$ grows stricly less then $g(n)$ or $f(n) < c \cdot g(n)$ for any value c. On the other hand for $O(g(n))$, $f(n)$ grows less than or equal to $g(n)$ or $f(n) \le c \cdot g(n)$ for some value c. This mean $O(g(n))$ has to satisfy one of two conditions to be true. It's $f(n)$ must grow either smaller to $c \cdot g(n)$ or it must grow equal to  it's $c \cdot g(n)$. If we look at the case $c=1$, it's $f(n)$ must grow either smaller to $g(n)$ or it must grow equal to  it's $g(n)$. As only one of these conditions must be true for $f(n)\in O(g(n))$ and the first condition is the same as $f(n)\in o(g(n))$, then it follows that $f(n)\in o(g(n)) \implies
f(n)\in O(g(n))$.

## Credits

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.