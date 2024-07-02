# How Did We Get Sicherman Dice?
_C.LaSota, 07/01/2024_

## Introduction

When you roll a standard pair of 6-sided dice, there are 36 possible outcomes.  However, if you're only interested in the _sum_ of the dice, there are only 11 possible values.  If you count the number of ways to obtain each sum, we end up with the following histogram:

| sum | # of ways |         dice combinations         |
| :-: | :-------: | :-------------------------------: |
|  2  |     1     |                1+1                |
|  3  |     2     |             1+2,  2+1             |
|  4  |     3     |          1+3,  2+2,  3+1          |
|  5  |     4     |       1+4,  2+3,  3+2,  4+1       |
|  6  |     5     |    1+5,  2+4,  3+3,  4+2,  5+1    |
|  7  |     6     | 1+6,  2+5,  3+4,  4+3,  5+2,  6+1 |
|  8  |     5     |    2+6,  3+5,  4+4,  5+3,  6+2    |
|  9  |     4     |       3+6,  4+5,  5+4,  6+3       |
| 10  |     3     |          4+6,  5+5,  6+4          |
| 11  |     2     |             5+6,  6+5             |
| 12  |     1     |                6+6                |

In 1978, George Sicherman discovered an alternative way to label the faces of a pair of 6-sided dice which would yield the *same* histogram for the possible sums.  His special pair of 6-sided dice have faces numbered as follows:

$\qquad\qquad\qquad$<strong style="color: #a00">die #1 : 1,  2,  2,  3,  3,  4</strong>$\qquad\qquad\qquad$ <strong style="color: #00a">die #2 :  1,  3,  4,  5,  6,  8</strong>

The histogram of sums for these dice is

| sum | # of ways |                                                                                                                                                                                                                                       dice combinations                                                                                                                                                                                                                                       |
| :-: | :-------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|  2  |     1     |                                                                                                                                                                                                         <strong style="color: #a00">1</strong>+<strong style="color: #00a">1</strong>                                                                                                                                                                                                         |
|  3  |     2     |                                                                                                                                                                 <strong style="color: #a00">2</strong>+<strong style="color: #00a">1</strong>,  <strong style="color: #a00">2</strong>+<strong style="color: #00a">1</strong>                                                                                                                                                                 |
|  4  |     3     |                                                                                                                         <strong style="color: #a00">1</strong>+<strong style="color: #00a">3</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">1</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">1</strong>                                                                                                                         |
|  5  |     4     |                                                                                 <strong style="color: #a00">1</strong>+<strong style="color: #00a">4</strong>,  <strong style="color: #a00">2</strong>+<strong style="color: #00a">3</strong>,  <strong style="color: #a00">2</strong>+<strong style="color: #00a">3</strong>,  <strong style="color: #a00">4</strong>+<strong style="color: #00a">1</strong>                                                                                 |
|  6  |     5     |                                         <strong style="color: #a00">1</strong>+<strong style="color: #00a">5</strong>,  <strong style="color: #a00">2</strong>+<strong style="color: #00a">4</strong>,  <strong style="color: #a00">2</strong>+<strong style="color: #00a">4</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">3</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">3</strong>                                         |
|  7  |     6     | <strong style="color: #a00">1</strong>+<strong style="color: #00a">6</strong>,  <strong style="color: #a00">2</strong>+<strong style="color: #00a">5</strong>,  <strong style="color: #a00">2</strong>+<strong style="color: #00a">5</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">4</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">4</strong>,  <strong style="color: #a00">4</strong>+<strong style="color: #00a">3</strong> |
|  8  |     5     |                                         <strong style="color: #a00">2</strong>+<strong style="color: #00a">6</strong>,  <strong style="color: #a00">2</strong>+<strong style="color: #00a">6</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">5</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">5</strong>,  <strong style="color: #a00">4</strong>+<strong style="color: #00a">4</strong>                                         |
|  9  |     4     |                                                                                 <strong style="color: #a00">1</strong>+<strong style="color: #00a">8</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">6</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">6</strong>,  <strong style="color: #a00">4</strong>+<strong style="color: #00a">5</strong>                                                                                 |
| 10  |     3     |                                                                                                                         <strong style="color: #a00">2</strong>+<strong style="color: #00a">8</strong>,  <strong style="color: #a00">2</strong>+<strong style="color: #00a">8</strong>,  <strong style="color: #a00">4</strong>+<strong style="color: #00a">6</strong>                                                                                                                         |
| 11  |     2     |                                                                                                                                                                 <strong style="color: #a00">3</strong>+<strong style="color: #00a">8</strong>,  <strong style="color: #a00">3</strong>+<strong style="color: #00a">8</strong>                                                                                                                                                                 |
| 12  |     1     |                                                                                                                                                                                                         <strong style="color: #a00">4</strong>+<strong style="color: #00a">8</strong>                                                                                                                                                                                                         |

Since all 36 possible outcomes of rolling Sicherman's pair of dice are equally probable, and they lead to the same probabilities for _sums_ of the dice, you could use his strange dice instead of the usual kind, and have all of the same *probabilities* for sums.  However, since his dice only provide 4 ways to obtain "doubles", they wouldn't be a suitable substitute in games where such outcomes were treated as special.

You're probably wondering how he figured this out.  You might even wonder if there exist other ways to re-label a pair of 6-sided dice to get the same histogram.  Well, Sicherman was able to use basic high-school algebra to _prove_ that his alternate relabeling was the only one that gave the same result for sums as a usual pair of 6-sided dice.  In this document, we will dive into the mathematics behind Sicherman's discovery.

## Dice notation

### Notation for common dice

In many tabletop games, a set of dice are used to imbue an element of chance into the outcomes of various game actions.  These dice typically have 4, 6, 8, 10, 12, or 20 sides, depending on the game, and have geometric shapes with high symmetry in an attempt to ensure that no one side will be favored when the dice are rolled.  The faces of such dice are usually labeled with integers from 1 to N, with N being the number of sides, and the labeling is usually done in way such that opposite faces sum to a value of N+1, no matter which pair of opposite faces are chosen.

Such "fair" dice are denoted with a small letter "**d**" followed by a number indicating the number of sides.  For example, a "**d6**" is usually a reference to a standard cube-shaped die, and "**d20**" usually refers to the 20-sided icosahedron shape commonly used in tabletop role-playing games.

### Notation for sums of dice

If we have to roll two or more dice, and add together the results of each die, then this will be denoted using either a plus sign "**+**" or an integer prefix if the dice are the same type.  So if a player rolls both a **d4** and a **d10**, and sums the results, then this is denoted as "**d4+d10**".  In a game like casino "craps", a player is required to roll a pair of **d6** dice.  Instead of denoting this as "d6+d6", it is simply written as "**2d6**".  If a game requires summing the results of rolling 5 cubical dice, this would be denoted as "**5d6**".  Summing the results of unusual dice combinations like a single **d6** and a pair of **d8** would be denoted as "**d6+2d8**".

### Generating functions

Instead of doing brute force tallies to determine the number of ways to get possible sums on combinations of dice, there's an alternative mathematical method that uses polynomials called **generating functions**.  In this method, a single **d6** would be represented by the following polynomial function:
$$d(x) = x + x^2 + x^3 + x^4 + x^5 + x^6$$
This representation works as follows.  Each _power_ of  $x$  in the polynomial corresponds to one possible face value of the **d6**.  You can see that $d(x)$ has all possible powers of $x$ from $x^1$ to $x^6$ , which tells us that the die being represented has all possible face values from 1 to 6.  In addition, the _coefficient_ of each power of  $x$  in the polynomial is interpreted as the *number of sides* of the die having the same face value corresponding to that power of $x$.  For $d(x)$ above, we can see that each power of  $x$  only has a coefficient of 1, which means that only one side has the value corresponding to each power of $x$.

Another extremely useful property of this generating function representation method is that since 1 raised to any power gives 1, then if we let $x=1$ in the polynomial function, it will give us the sum of the coefficients.  Since the coefficients tell us how many sides there are for each face value, then the sum of the coefficients is equal to the total number of sides that the die has.  What this means is that, by letting $x=1$ in the polynomial, it tells us the number of possible outcomes.  So if we let $x=1$ in  $d(x)$ above, then we obtain 6 -- as we should, since there are 6 possible outcomes for a d6.

The first of Sicherman's dice given previously would be represented by the following generating function polynomial, which we'll call $p(x)$:
$$p(x) = x + 2x^2 + 2x^3 + x^4 
$$
Note that the powers of $x$ in this polynomial are 1, 2, 3, and 4.  This means that the possible face values of this die are 1, 2, 3, and 4.  However, since the coefficient of  $x^2$  is 2, this means that there are *two* sides that have a face value of 2.  Likewise, since the coefficient of $x^3$ is 2, there are also *two* sides that have a face value of 3.  However, there is only one side having a value of 1, and one side having a value of 4.  If we let $x=1$ , we can see that the value of $p(1)$ is equal to 6, which means that we have a 6-sided die.

Ok, so why are we using ploynomials to represent dice?

### Using generating functions for sums of dice outcomes

The power of this generating function representation method shows its strength when we wish to consider the possible *sums* for two (or more) dice.

We can find the number of ways to obtain _sums_ for 2d6 by taking the polynomial  $d(x)$ above and multiplying it by itself (i.e. **squaring** it):
$$\begin{align}d(x)\cdot d(x) = [~d(x)~]^2 &= (x + x^2 + x^3 + x^4 + x^5 + x^6)\cdot(x + x^2 + x^3 + x^4 + x^5 + x^6) \\
&= x^2 + 2x^3 + 3x^4 + 4x^5 + 5x^6 + 6x^7 + 5x^8 + 4x^9 + 3x^{10} + 2x^{11} + x^{12}
\end{align}$$
Recall that when we multiply polynomials together, we form all possible products, and then simplify the result by grouping together terms that have the same power of $x$ and summing their coefficients.  This has the effect of essentially counting the number of ways to obtain each particular power of $x$.  *This is exactly what we want!*

Interpreting the result above for $[~d(x)~]^2$, it's as if we had a _single_ 36-sided die, but where the numbers on the faces are the possible _sums_ of 2d6.  It tells us that for such a die... 

   ... one side had a value of 2,
   ... 2 sides had a value of 3,
   ... 3 sides had a value of 4,
   ... 4 sides had a value of 5,
   ... 5 sides had a value of 6,
   ... 6 sides had a value of 7,
   ... 5 sides had a value of 8,
   ... 4 sides had a value of 9,
   .. .3 sides had a value of 10,
   ... 2 sides had a value of 11,
... and one side had a value of 12.

Notice that if we let $x=1$ in our result for  $[~d(x)~]^2$, then we get a value of 36, as expected, since d(1)=6 and we're squaring it.  So this method counts the number of possible outcomes for the *pair* of d6 dice, giving 36 as expected.

## Sicherman dice

Recall that Sicherman's special pair of 6-sided dice have faces numbered as follows:

$\qquad\qquad\qquad$<strong style="color: #a00">die #1 : 1,  2,  2,  3,  3,  4</strong>$\qquad\qquad\qquad$ <strong style="color: #00a">die #2 :  1,  3,  4,  5,  6,  8</strong>

Using the generating function method, we can consider the possible outcomes for the *sum* of these special dice.  Let  $p(x)$  represent die #1, and let  $q(x)$  represent die #2: $$\begin{align} p(x) &= x + 2x^2 + 2x^3 + x^4 \\
& \\
q(x) &= x + x^3 + x^4 + x^5 + x^6 + x^8 \end{align}$$Now we do the same thing as before -- create the product of these two polynomials:
$$\begin{align} p(x)\cdot q(x) ~&=~ (x + 2x^2 + 2x^3 + x^4)\cdot(x + x^3 + x^4 + x^5 + x^6 + x^8) \\
&=~ x^2 + 2x^3 + 3x^4 + 4x^5 + 5x^6 + 6x^7 + 5x^8 + 4x^9 + 3x^{10} + 2x^{11} + x^{12}

\end{align}$$
Note the amazing result!  This is the _same polynomial_ as we obtained for $[d(x)]^2$.

This means that if you only care about the _sum_ of a pair of 6-sided dice, you can either use a standard 2d6, or, you can use Sicherman's dice to end up with the same results for sums.

At this point you might be wondering if there are additional ways to label a pair of 6-sided dice to get the same result for sums.  Well, if we insist that the labels are always positive integers, the answer is "no".  Sicherman's dice are the **only** alternate labeling of faces of a pair of d6 so that it yields the same probability for sums as 2d6.  We can use the generating function method and little more algebra to see why.

### The mathematics behind Sicherman dice

The reason for the existence of an alternate way of labeling a pair of d6 dice to obtain the same histogram for the dice sums as 2d6 comes down to the _factorization_ of the generating function polynomials we introduced.

The generating function  $d(x)$  we used for a single ordinary **d6** die can be _completely factored_ into the product of smaller polynomials:
$$\begin{align} d(x) ~&=~ x + x^2 + x^3 + x^4 + x^5 + x^6 \\
&=~ x\,(1 + x + x^2 + x^3 + x^4 + x^5) \\
&=~ x\,(1 + x)\,(1 + x^2 + x^4) \\
&=~ x\,(1 + x)\,(1 + x + x^2)\,(1 - x + x^2)
\end{align}$$
We say that $d(x)$ is "completely" factored, because each of the polynomial factors cannot be factored any further.  The most important aspect of this "complete" factorization is that it is **unique**.  There is no other way to completely factor the polynomial we started with.

This is kind of like completely factoring a whole number, say 42, into a product of prime numbers:$$42 = 1 * 2 * 3 * 7$$
If we consider the generating function $[~d(x)~]^2$  for the sum of 2d6, then we must square the factors of $d(x)$ to get a complete factorization of $[~d(x)~]^2$:
$$ [~d(x)~]^2 ~=~ x^2\,(1 + x)^2\,(1 + x + x^2)^2\,(1 - x + x^2)^2$$
The clever thing Sicherman did was to _split_ these factors into two sets, where each set produced one of the two polynomials you saw above:
$$\begin{align} [d(x)]^2 &= p(x)\cdot q(x) \\
p(x) ~&=~ x\,(1 + x)\,(1 + x + x^2) &~=~ x + 2x^2 + 2x^3 + x^4 \quad\quad\quad~\\
q(x) ~&=~ x\,(1 + x)\,(1 + x + x^2)\,(1 - x + x^2)^2 ~&=~ x + x^3 + x^4 + x^5 + x^6 + x^8
\end{align}$$
The analogy here would be like factoring the square of 42 into the product of two numbers, where each number was created by regrouping the squares of the prime factors of 42:
$$\begin{align} 42\cdot 42 &= 1^2\cdot 2^2\cdot 3^2\cdot 7^2\\
&= (1\cdot 2\cdot 3)(1\cdot 2\cdot 3\cdot 7\cdot 7\cdot) \\
&= 6 \cdot 294\end{align}$$
Because it's going to be important to the argument below, remember that letting $x=1$ in each representative polynomial just counts the sides/outcomes of the die being represented by that polynomial.  Doing this here gives  $p(1) = 6$  and  $q(1) = 6$, confirming that Sicherman's factorization does indeed result in a pair of 6-sided dice.

### The uniqueness of Sicherman dice

Suppose we hope to find yet another alternate way of labeling a pair of 6-sided dice to give the same sum distribution as 2d6 .  How would we do this?

Well, there's a somewhat trivial way to produce a new labeling for pair of 6-sided dice by adding a 1 to every face of one d6, and subtracting a 1 from every face of another d6.  This would mean one die would have face values from 2 to 7, and the other die would have face values from 0 to 5.  If we consider the generating functions for such dice, we would have

$\qquad\qquad r(x) ~=~ x^2 + x^3 + x^4 + x^5 + x^6 + x^7 \qquad\qquad\qquad s(x) ~=~ 1 + x + x^2 + x^3 + x^4 + x^5$

Note that the single "1" term in the $s(x)$ polynomial means one die would have a single face with a value of 0 (since $1 = 1 \cdot x^0$ ).  But notice that all that's happened here is that  $d(x)$ was multiplied by  $x$  to give $r(x)$, and $d(x)$ was divided by $x$ to yield $s(x)$.  So naturally, we should expect that the product of $r(x)$ and $s(x)$ will give us $[~d(x)~]^2$.

If we factor these polynomials, we obtain
$$\begin{align} r(x) ~&=~ x^2 + x^3 + x^4 + x^5 + x^6 + x^7 &=~ x^2\,(1+x)\,(1 + x + x^2)\,(1 - x + x^2)\\
s(x) ~&=~ 1 + x + x^2 + x^3 + x^4 + x^5 &=~ (1+x)\,(1+x+x^2)\,(1-x+x^2)\quad
\end{align}$$
Notice that the factorizations of $r(x)$ and $s(x)$ on the right above are just the same factors from $[~d(x)~]^2$  we saw earlier!   So we confirm that indeed, 
$$\begin{align} r(x)\cdot s(x) &=~ x^2\,(1+x)^2\,(1 + x + x^2)^2\,(1 - x + x^2)^2\\
 ~&=~ [~d(x)~]^2
\end{align}$$
So we see that this trivial shift of the face values up and down by 1 on two d6 dice result is just a slightly different way of partitioning the factors of $[d(x)]^2$  than we saw with $p(x)$ and $q(x)$ in the previous section.  Substitution of $x=1$ still results in $r(1)=6$ and $s(1)=6$, showing that they both still represent 6-sided dice.

However, this shifting method of coming up with an alternative numbering is somewhat unsatisfactory when we consider how surprising Sicherman's labeling is.  So let's focus on finding an alternate labeling where the face values are only _positive_ integers.  Doing so, means that when we split up the factors of $[d(x)]^2$ into two polynomials, neither polynomial can contain a "1" term -- all of the terms will contain some positive power of $x$.

So what we need to do is come up with another way to take the factors of $[d(x)]^2$ and separate them such that they form 2 different polynomials, but do it in a way so that they _both_ equal 6 when we let $x=1$, because we want each of the two dice to be 6-sided cubes just like a d6.

So we're searching for two polynomials $f(x)$ and $g(x)$ such that:
$$[d(x)]^2 = f(x)\cdot g(x)$$where
$$f(1)=6 \quad \mathrm{and} \quad g(1)=6$$
If we look at the factors of $[d(x)]^2$ we obtained earlier, and imagine letting $x=1$ for each of them, we can see that we generate a set of prime factors of 36.
$$\begin{align} [d(x)]^2 ~&=~ x^2\,(1 + x)^2\,(1 + x + x^2)^2\,(1 - x + x^2)^2 \\
[d(1)]^2 &= 1\cdot 1\cdot 2\cdot 2\cdot 3\cdot 3\cdot 1\cdot 1
\end{align}
$$

We want to regroup these factors among $f(x)$ and $g(x)$ such they they individually multiply up to a value of 6 when we let $x=1$.  This forces $f(x)$ and $g(x)$ to each contain the terms $(1+x)$ and $(1+x+x^2)$  because they equal 2 and 3, respectively.  When we let $x=1$:
$$\begin{align}
f(x) &= (1 + x)(1 + x + x^2)(\text{other factors that equal 1 when } x=1) \\
g(x) &= (1 + x)(1 + x + x^2)(\text{other factors that equal 1 when } x=1)
\end{align}$$
Because we said we wanted each of the dice to have positive integers for its face values, this means that both $f(x)$ and $g(x)$ have to be polynomials whose lowest power of $x$ is just $x$ itself.  This forces $f(x)$ and $g(x)$ to each contain $x$ as a factor.  So now we have
$$\begin{align}
f(x) &= x(1 + x)(1 + x + x^2)(\text{remaining factor(s) that equal 1 when } x=1) \\
g(x) &= x(1 + x)(1 + x + x^2)(\text{remaining factor(s) that equal 1 when } x=1)
\end{align}$$
The only factors remaining to assign to $f(x)$ and/or $g(x)$ are two factors of $(1-x+x^2)$.  We can see that there are only two unique ways to do this.  Either each polynomial gets one factor of $(1-x+x^2)$, or one of the polynomials get two factors and the other gets none.  So we only have two possible types of results for $f(x)$ and $g(x)$.  Either
$$\begin{align}
f(x) &= d(x) = x(1 + x)(1 + x + x^2)(1 - x + x^2) ~=~ x+x^2+x^3+x^4+x^5+x^6\\
g(x) &= d(x) = x(1 + x)(1 + x + x^2)(1 - x + x^2) ~=~ x+x^2+x^3+x^4+x^5+x^6
\end{align}$$
or
$$\begin{align}
f(x) &= x(1 + x)(1 + x + x^2)(1 - x + x^2)^2 ~=~ x+x^3+x^4+x^5+x^6+x^8\\
g(x) &= x(1 + x)(1 + x + x^2) \qquad\qquad\quad\,\,\, ~=~ x+2x^2+2x^3+x^4
\end{align}$$
Note that the first case is the just the classic 2d6 pair of dice, where both dice are the same, each having six sides numbered 1 through 6.  The second case is Sicherman's result.  Since these are the only two possible factorizations of $[d(x)]^2$ that give polynomials which evaluate to 6 when $x=1$, and which have $x^1$ as the lowest power of $x$ in each, then we've just shown that there are no other possible labelings of a pair of 6-sided dice which will produce the same histogram for the _sums_ of the values of the pair of dice!

------------------------------------------------------
### Homework for the Curious:

1. Write down the generating function for a single d8.  Check your result by letting $x=1$ to obtain the number of possible outcomes.
2. How many ways can you get a sum of 10 when rolling 2d8?
3. How many ways can you get a sum of 7 when rolling 3d4?
4. How many ways can you get a sum of 9 when rolling 6d2 (this is like flipping 6 coins where "tails"=1 and "heads"=2)?
5. Show that you can factor the generating function for a single d10 into the product of three polynomials, one of which is just "$x$" by itself.  Show that the other two factors equal 2 and 5 when you let $x=1$.
6. Show that your answer to #1 can be factored as $x(1+x)(1+x^2)(1+x^4)$.
7. _(Challenge)_ Produce **three** additional possible alternative labeling schemes for a pair of 8-sided dice that will each give the same histogram for sums as the usual 2d8.
   
### Answers to Homework
1. Since a **d8** has eight sides, and all values from 1 to 8 show up on the faces, then a generating function $q(x)$ representing it needs to have every single power of $x$ from $x^1$ to $x^8$, and where the coefficient of each power is only 1.  Therefore: $$~q(x) = x+x^2+x^3+x^4+x^5+x^6+x^7+x^8.$$When $x=1$, then $q(1)=8$ as it should.
   
2. When representing the results of _sums_ of dice, we form a product of the generating function for each of the dice involved.  Since we are considerind a _pair_ of **d8**, then we multiply our answer from question #1 above by itself, simplify, and look at the coefficients of each power of $x$.  The coefficient tells us how many ways the sum corresponding to that power can be formed.  So we create $[~q(x)~]^2$, and then we find the coefficient of $x^{10}$ : $$\begin{align} &[~q(x)~]^2 = (x + x^2+x^3+x^4+x^5+x^6+x^7+x^8)\cdot (x+x^2+x^3+x^4+x^5+x^6+x^7+x^8) \\ =\, & x^2 + 2x^3 + 3x^4 + 4x^5 + 5x^6 + 6x^7 + 7x^8 + 8x^9 + 7x^{10} + 6x^{11} + 5x^{12} + 4x^{13} + 3x^{14} + 2x^{15} + x^{16} \end{align}$$ The coefficient of $x^{10}$ is 7, so there are **7** ways to get a sum of 10 from 2d8.
   
3. Represent a single **d4** by $h(x) = x+x^2+x^3+x^4$  and find the coefficient of $x^7$  in the product $[~h(x)~]^3$ :  $$\begin{align}[~h(x)~]^3 &= (x+x^2+x^3+x^4)\cdot (x+x^2+x^3+x^4)\cdot (x+x^2+x^3+x^4) \\ &= (x+x^2+x^3+x^4)\cdot (x^2 + 2x^3 + 3x^4 + 4x^5 + 3x^6 + 2x^7 + x^8) \\ &= x^3 + 3x^4 + 6x^5 + 10x^6 + 12x^7 + 12x^8 + 10x^9 + 6x^{10} + 3x^{11} + x^{12}  \end{align}$$The coefficient of $x^7$ is 12, so there are **12** ways to get a sum of 7 from 3d4.
   
4. Represent a single **d2** by $x+x^2$ and find the coefficient of $x^9$ in the product $[~x+x^2~]^6$  : $$\begin{align}[~x+x^2~]^6 &= [~x(1+x)~]^6 \\ &= x^6~[1+x]^6 \\ &= x^6~[1 + 6x + 15x^2 + 20x^3 + 15x^4 + 6x^5 + x^6~] \\ &= x^6 + 6x^7 + 15x^8 + 20x^9 + 15x^{10} + 6x^{11} + x^{12} \end{align}$$Here we took advantage of the _binomial theorem_ to quickly expand $(1+x)^6$.  The coefficient of $x^9$ in the result is 20, so there are **20** ways to get a sum of 9 from 6d2.
   
5. A single d10 can represented as a generating function we will call $T(x)$.  We can factor $T(x)$ by doing some grouping of terms: $$\begin{align}T(x) &= x + x^2 + x^3 + x^4 + x^5 + x^6 + x^7 +x ^8 +x^9 +x^{10} \\ &= x\cdot(1 + x + x^2 + x^3 + x^4 + x^5 + x^6 + x^7 +x ^8 +x^9)  \\ &= x\cdot [~(1 + x + x^2 + x^3 + x^4) +~ x^5(1 + x + x^2 + x^3 +x ^4)~] \\ &= x\cdot(1 + x^5)\cdot(1 + x + x^2 + x^3 + x^4)\end{align} $$When we let $x=1$, then $(1+x^5) = 2$  and  $(1+x+x^2+x^3+x^4) = 5$, so that  $T(1)=10$.
   
6. We factor $q(x)$ as given in our answer to problem #1.  We do this by performing multiple grouping steps like we did in the answer to problem #5 : $$\begin{align}~q(x) &= x+x^2+x^3+x^4+x^5+x^6+x^7+x^8 \\ &= x\cdot [~ 1+ x + x^2 + x^3 + x^4 + x^5 + x^6 + x^7~] \\ &= x\cdot[~(1 + x + x^2 + x^3) + x^4(1 + x + x^2 + x^3)~] \\ &= x\cdot (1+x^4)\cdot [~1+x+x^2+x^3~] \\ &= x\cdot (1+x^4)\cdot [~(1+x) + x^2(1+x)~] \\ &= x\cdot (1+x^4)\cdot (1+x^2)\cdot (1+x)\end{align}$$Note that when $x=1$, then $q(1) = 1\cdot 2\cdot 2\cdot 2 = 8$  as expected.
   
7. We've already seen the expanded expression for $[~q(x)~]^2$ in the answer to problem #2 above.  But when we express it in terms of its factors from our answer to problem #6, we get: $$\begin{align}[~q(x)~]^2 =  x^2~(1+x)^2~(1+x^2)^2~(1+x^4)^2\end{align}$$In order to find alternate labelings of a _pair_ of d8, then we need to do what Sicherman did for a pair of d6 -- we need to regroup these factors into a pair of polynomials.  However, we are insisting that each of the polynomials we produce equals 8 when we let $x=1$, because each polynomial is supposed to represent an 8-sided die.  To get started, we notice that letting $x=1$ in $[~q(x)~]^2$ above tells us that each term contributes a 1 or a 2 to the full product: $$\begin{align}[~q(1)~]^2 =  1\cdot 1\cdot 2 \cdot 2 \cdot 2 \cdot 2 \cdot 2 \cdot 2 \end{align}$$So we want to create two polynomials, $f(x)$ and $g(x)$, such that $f(x)\cdot g(x)=[~q(x)~]^2$.  But we also have two constraints.  First, we want each of the dice face values to be positive.  This means both $f(x)$ and $g(x)$ must _each_ be given a single factor of $x$ from the two available.  Second, we want each die to have 8 sides.  So this means that we have to split our factors up in such a way so that when $x=1$, we get $$f(1) = 1\cdot 2\cdot 2\cdot 2 = 8 \qquad\text{and}\qquad g(1) = 1\cdot 2\cdot 2\cdot 2 = 8$$It turns out that there are 4 ways to do this.  One way is the usual way that d8 dice are labeled.  Boring!  But another way is the following :$$\begin{align}f(x) &= x(1+x)(1+x^2)^2 = x+x^2+2x^3+2x^4+x^5+x^6\\ g(x) &= x(1+x)(1+x^4)^2 = x+x^2+2x^5+2x^6+x^9+x^{10}\end{align}$$This yields one 8-sided die with faces 1, 2, 3, 3, 4, 4, 5, and 6, and a second 8-sided die having faces 1, 2, 5, 5, 6, 6, 9, and 10.  Try it out -- it works!!!  Another alternate labeling uses a different distribution of factors : $$\begin{align}f(x) &= x(1+x^2)(1+x)^2 = x+2x^2+2x^3+2x^4+x^5\\ g(x) &= x(1+x^2)(1+x^4)^2 = x+x^3+2x^5+2x^7+x^9+x^{11}\end{align}$$This gives one 8-sided die with faces 1, 2, 2, 3, 3, 4, 4, and 5, and a second 8-sided die having faces 1, 3, 5, 5, 7, 7, 9, and 11.  Take note that this labeling scheme isn't just some shift of the previous one.  It's unique and it works.  Finally, the last non-standard alternate labeling scheme uses yet another way to distribute the factors : $$\begin{align}f(x) &= x(1+x^4)(1+x)^2 = x+2x^2+x^3+x^5+2x^6+x^7\\ g(x) &= x(1+x^4)(1+x^2)^2 = x+2x^3+2x^5+2x^7+x^9\end{align}$$This last labeling scheme gives an 8-sided die with faces 1, 2, 2, 3, 5, 6, 6, and 7, and a second die having faces 1, 3, 3, 5, 5, 7, 7, and 9.  Again, notice that this isn't just some trivial shift of either of the two non-standard labelings we've produced so far.
   