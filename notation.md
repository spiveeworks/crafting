
#Process
Ingredients (time)=Capital=> Products
or
Ingredients =Capital=> Products

e.g.
egg (5 minutes)=Frying pan, Chef=> fried egg

Note the resemblence to a chemical equation. For this reason ingredients and products may be separated with a + sign

flint + rope + branch (5 minutes)=Survivalist=> tool + twig shrapnel

also note that due to the complications of capital and time, applying algebra, and cancelling elements that are 
both ingredients and products, are not sensible. Expectations are the basic way of getting past this, but a system for
more complex calculations involving capital and time may be described in the future.

#Expectation

These represent some information about a process, in order to make them more manipulable.

Ingredients -> Products

e.g.
egg -> fried egg
flint + rope + branch -> tool + twig shrapnel

Using these more restrictive representations, many simple deductions can be made.

If it is known that A -> B is a valid expectation, and C -> D is also, then:
A + C -> B + D

If A + B -> A + C
then A -> C (cancellation)

Scalar multiplication by any rational number is also allowed:
if nA -> nB
then mA -> mB

From these many obvious conclusions can be made:

A -> B, B -> C
therefore A + B -> B + C
therefore A -> C (transitive rule)

A + B -> C
C + D -> B + E
therefore A + B + C + D -> B + C + E
therefore A + D -> E
In this example B is a capital good even though it appears as an ingredient in some of the steps.

#Reduction

It will be noted that
A + B (x)=> B + C
is equivalent to
A (x)=B=> C

A process is reduced if such 'B terms' have all been moved to the Capital section of the notation.

An expectation can potentially be reduced in a number of ways:
First of all the cancellation rule must be applied until no term appears on both sides of the expectation.

An expectation is redundancy reduced if it has no ingredient that is also a product.

An expectation is monically reduced if the first product listed has no coefficient, 
and it is redundancy reduced.

An expectation is naturally reduced if all coefficients are whole numbers, 
the highest common factor of them all is 1, 
and it is redundancy reduced.

#Abstract Ingredients

Abstract ingredients are a way of reducing redundancy in processes and expectations.

They are specified by lines of the form:
identifier ::= ingredients - balancing_ingredients
e.g.
water in a bucket ::= bucket of water - empty bucket

if Q ::= Y - X
then A + Y =B=> C + X
is equivalent to A + Q =B=> C
and A + X =B=> C + Y
is equivalent to A =B=> C + Q
(If multiple definitions of Q are given then this logic doesn't always apply backwards, be careful)

Multiple definitions can be given.
Any process with an abstract ingredient must be true of any possible substitution
Either ingredients or balancing_ingredients can be empty, and if balancing_ingredients is empty then the - should be removed.

Note that if an identifier, Q say, has multiple definitions, then
Q + Q + A => B
doesn't mean the same thing as
2Q + A => B
although the former implies the latter.

Also note that Q + A => Q + B
is distinct from A =Q=> B
in two ways:

First if Q has multiple definitions, the former specifies that any Q plus A can make any other Q plus B
This would then imply the latter, which says that A can be made into B using any Q, without consuming or changing said Q.

Second if Q has base_ingredients listed, then the former specifies that A can be turned into B while undoing one Q action, and doing another.
This would still imply the latter, which now says that both the ingredients of some Q, *and* the base ingredients of that same Q, are both required but not consumed by the process.
