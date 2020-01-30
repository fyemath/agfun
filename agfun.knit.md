--- 
title: "Algebra and Geometry of Elementary Functions"
author: "Fei Ye"
date: "2020-01-29"
site: bookdown::bookdown_site
documentclass: latex/elegantbookr
# bibliography: [book.bib]
# biblio-style: apalike
# logo: "figure/logo.png"
# cover: "figure/cover.jpg"
institute: ""
extrainfo: ""
version: "0.01"
github-repo: fyemath/agfun
classoption: "en,12pt"
# indent: 40pt
# subparagraph: yes
description: "This notebook is designed to give a concise introduction to algebra and geometry of elementary functions which can be served as a textbook for a College Algebra course."
---

# Introduction {-}

This notebook is intended to give a brief introduction to elementary functions emphasizing on effective thinking in algebra and geometry.

In the first part, we will review mathematical operations including addition, multiplication, $n$-th root, exponentiation and logarithm.

In the second part, we will study the concepts of functions, algebraic functions and their applications.

In the third part, we will study elementary transcendental functions and applications.

Comments and suggestions are very welcome.

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

![by-nc-sa license icon](figs/by-nc-sa.png)

<!--chapter:end:index.Rmd-->

# (PART\*) Part I: Mathematical Operations {-}

# Integer Exponents

## Don't Be Tricked

\BeginKnitrBlock{rmdthink}<div class="rmdthink">
A pizza shop sales 12-inches pizza and 8-inches pizza at the price \$12/each and \$6/each respectively.  With \$12, would you like to order one 12-inches and two 8-inches. Why?
</div>\EndKnitrBlock{rmdthink}

\BeginKnitrBlock{rmdthink}<div class="rmdthink">
A sheet of everyday copy paper is about 0.01 millimeter thick. Repeat folding along a different side 20 times. Now, how thick do you think the folded paper is?
</div>\EndKnitrBlock{rmdthink}

## Properties of Exponents
For an integer $n$, and an expression $x$, the mathematical operation of the $n$-times repeated multiplication of $x$  is call exponentiation, written as $x^n$, that is,
$$
x^n=\underbrace{x\cdot x \cdots x}_{n \text{factors of} x}.
$$


In the notation $x^n$, $n$ is called ***the exponent***, $x$ is called ***the base***, and $x^n$ is called ***the power***, read as "$x$ raised to the $n$-th power",  "$x$ to the $n$-th power", "$x$ to the $n$-th", "$x$ to the power of $n$" or "$x$ to the $n$".

| Property | Example|
|---|---|
|The product rule $$x^m\cdot x^n=x^{m+n}.$$ | $$2x^2\cdot (-3x^3)=-6x^5.$$ |
| The quotient rule (for $x\neq 0$.) $$\dfrac{x^m}{x^n}= \begin{cases} x^{m-n}  & \text{if} m\ge n.\\[1em] \dfrac{1}{x^{n-m}} & \text{if} m\le n. \end{cases} $$ | $$\frac{15x^5}{5x^2}=3x^3;$$ $$\frac{-3x^2}{6x^3}=-\frac{1}{2x}.$$ |
| The zero exponent rule (for $x\neq 0$.) $$x^0=1.$$ | $$(-2)^0=1;$$ $$-x^0=-1.$$ |
| The negative exponent rule (for $x\neq 0$.) $$x^{-n}=\dfrac{1}{x^n} \quad\text{and}\quad \dfrac{1}{x^{-n}}=x^n.$$ | $$(-2)^{-3}=\frac{1}{(-2)^3}=-\frac18;$$ $$\frac{x^{-2}}{x^{-3}}=\frac{x^3}{x^2}=x.$$ |
| The power to a power rule $$\left(x^a\right)^b=x^{ab}.$$ | $$\left(2^{2}\right)^3=2^6=64;$$ $$\left(x^2\right)^3=x^6.$$ |
| The product raised to a power rule $$(xy)^n=x^ny^n.$$ | $$\left(-2x\right)^{2}=(-2)^2x^2=4x^2.$$ |
| The quotient raised to a power rule (for $y\neq 0$.) $$\left(\dfrac{x}{y}\right)^n=\dfrac{x^n}{y^n}.$$ | $$    \left(\dfrac{x}{-2}\right)^{3}=\dfrac{x^3}{(-2)^3}=-\dfrac{x^3}{8}.$$ |

\BeginKnitrBlock{rmdnote}<div class="rmdnote">
**Order of Basic Mathematical Operations**

In mathematics, the order of operations reflects conventions about which procedure should be performed first. There are four levels (from the highest to the lowest):

**Parenthesis**; **Exponentiation**; **Multiplication and Division**; **Addition and Subtraction**.

Within the same level, the convention is to perform from the left to the right.
</div>\EndKnitrBlock{rmdnote}

## Examples

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-4"><strong>(\#exm:unnamed-chunk-4) </strong></span>
Simplify. **Write with positive exponents.**
$$
\left(\dfrac{2y^{-2}z^{-5}}{4x^{-3}y^6}\right)^{-4}.
$$
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
$$
\left(\dfrac{2y^{-2}z^{-5}}{4x^{-3}y^6}\right)^{-4}
=\left(\dfrac{x^3}{2z^{5}y^8}\right)^{-4}
=\left(\dfrac{2z^{5}y^8}{x^3}\right)^4
=\dfrac{2^4(z^{5})^4(y^8)^4}{(x^3)^4}
=\dfrac{16y^{32}z^{20}}{x^{12}}.
$$
</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{rmdtip}<div class="rmdtip">
**Simplify (at least partially) the problem first**

To avoid mistakes when working with negative exponents, it's better to apply the negative exponent rule to change negative exponents to positive exponents and simplify the base first.
</div>\EndKnitrBlock{rmdtip}

## Practice

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-7"><strong>(\#exr:unnamed-chunk-7) </strong></span>
Simplify. **Write with positive exponents.**

1. $(3a^2b^3c^2)(4abc^2)(2b^2c^3)$
1. $\dfrac{4y^3z^0}{x^2y^2}$
1. $(-2)^{-3}$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-8"><strong>(\#exr:unnamed-chunk-8) </strong></span>
Simplify. **Write with positive exponents.**

1. $\dfrac{-u^0v^{15}}{v^{16}}$
1. $(-2a^3b^2c^0)^3$
1. $\dfrac{m^5 n^{2}}{(mn)^3}$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-9"><strong>(\#exr:unnamed-chunk-9) </strong></span>
Simplify. **Write with positive exponents.**

1. $(-3a^2x^3)^{-2}$
1. $\left(\dfrac{-x^0y^3}{2wz^2}\right)^3$
1. $\dfrac{3^{-2}a^{-3}b^5}{x^{-3}y^{-4}}$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-10"><strong>(\#exr:unnamed-chunk-10) </strong></span>
Simplify. **Write with positive exponents.**

1. $\left(-x^{-1}(-y)^2\right)^3$
2. $\left(\dfrac{6x^{-2}y^5}{2y^{-3}z^{-11}}\right)^{-3}$
3. $\dfrac{(3 x^{2} y^{-1})^{-3}(2 x^{-3} y^{2})^{-1}}{(x^{6} y^{-5})^{-2}}$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-11"><strong>(\#exr:unnamed-chunk-11) </strong></span>
A store has large size and small size watermelons. A large one cost \$4 and a small one \$1. Putting on the same table, a smaller watermelons has only half the height of the larger one. Given \$4, will you buy a large watermelon or 4 smaller ones? Why?
</div>\EndKnitrBlock{exercise}

<!--chapter:end:101-Integer-Exponents.Rmd-->

# Review of Factoring

## Can You Beat a Calculator

\BeginKnitrBlock{rmdthink}<div class="rmdthink">
Do you know a faster way to find the values?

1. Find the value of the polynomial $2x^3-98x$ when $x=-7$.

2. Find the value of the polynomial $x^2-9x-22$ when $x=11$.

3. Find the value of the polynomial $x^3-2x^2-9x+18$ when $x=-3$.

4. Find the value of $16^2-14^2$.
</div>\EndKnitrBlock{rmdthink}

## Factor by Removing the GCF

***The  greatest common factor (GCF)*** of two terms is a polynomial with the **greatest coefficient** and of the **highest possible degree** that divides each term.

To ***factor a polynomial*** is to **express the polynomial as a product** of polynomials of lower degrees. The first and the easiest step is to factor out the GCF of all terms.

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-13"><strong>(\#exm:unnamed-chunk-13) </strong></span>
Factor $4x^3y-8x^2y^2+12x^3y^3$.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Find the GCF of all terms.  
   The GCF of $4x^3y$, $-8x^2y^2$ and $12x^4y^3$ is $4x^2y$.

2. Write each term as the product of the GCF and the remaining factor.  
   $4x^3y=(4x^2y)\cdot x$, $-8x^2y^2=(4x^2y)\cdot (-2y)$, and $12x^4y^3=(4x^2y)(3xy^2)$.

3. Factor out the GCF from each term.  
   $4x^3y-8x^2y^2+12x^3y^3=4x^2y\cdot(x-2y+3xy^2)$.
</div>\EndKnitrBlock{solution}

## Factor by Grouping

For a four-term polynomial, in general, we will group them into two groups and factor out the GCF for each group and then factor further.

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-15"><strong>(\#exm:unnamed-chunk-15) </strong></span>
Factor $2x^2-6xy+xz-3yz$.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Group the first two terms and the last two terms.
   $$
    \begin{aligned}
    &2x^2-6xy+xz-3yz\\
    =&(2x^2-6xy)+(xz-3yz)
    \end{aligned}
   $$
   
2. Factor out the GCF from each group.  
   $$
    \begin{aligned}
    =&2x(x-3y)+z(x-3y)
    \end{aligned}
   $$

3. Factor out the binomial GCF.
$$
\begin{aligned}
=&(x-3y)(2x+z).
\end{aligned}
$$
</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-17"><strong>(\#exm:unnamed-chunk-17) </strong></span>
Factor $ax+4b-2a-2bx$.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Group the first term with the third term and group the second term with the last term.
$$
\begin{aligned}
&ax+4b-2a-2bx\\
=&(ax-2a)+(-2bx+4b)
\end{aligned}
$$

2. Factor out the GCF from each group.
$$
\begin{aligned}
=&a(x-2)+(-2b)(x-2)
\end{aligned}
$$

3. Factor out the binomial GCF.
$$
\begin{aligned}
=&(x-2)(a-2b).
\end{aligned}
$$
</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{rmdtip}<div class="rmdtip">
**Guess and check.**  
Once you factored one group, you may expect that the other group has the same binomial factor so that factoring may be continued.
</div>\EndKnitrBlock{rmdtip}

## Factor Difference of Powers

Factoring is closely related to solving polynomial equations. If a polynomial equation $p(x)=0$ has a solution $r$, then $p(x)$ has a factor $x-r$. For example, $x^n-r^n=0$ has a solution $x=r$. So the difference $x^n-r^n$ has a factor $(x-r)$. Using long division or by induction, we obtain the following equality.

**Difference of $n$-th powers**

$$a^n-b^n=(a-b)(a^{n-1}+a^{n-2}b+\cdots +ab^{n-2}+b^{n-1})$$

In particular,

$$a^2-b^2=(a-b)(a+b).$$

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-20"><strong>(\#exm:unnamed-chunk-20) </strong></span>
Factor $25x^2-16$.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Recognize the binomial as a difference of squares.
$$\begin{aligned}
&25x^2-16\\
=&(5x)^2-4^2
\end{aligned}
$$

2. Apply the formula.
$$
\begin{aligned}
=&(5x-4)(5x+4).
\end{aligned}
$$
</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-22"><strong>(\#exm:unnamed-chunk-22) </strong></span>
Factor $32x^3y-2xy^5$ completely.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
$$
32x^3y-2xy^3=2xy(16x^2-y^4)=2xy((4x)^2-(y^2)^2)=2xy(4x+y^2)(4x-y^2).
$$
</div>\EndKnitrBlock{solution}

## Factor Trinomials

If a trinomial $ax^2+bx+c$, $A\neq 0$, can be factored, then it can be expressed as a product of two binomials: 
$$ax^2+bx+c=(mx+n)(px+q).$$
By simplify the product using the FOIL method and comparing coefficients, we observe that 
$$
a=\underbrace{mn}_{\mathrm{F}}\quad\quad\quad
b=\underbrace{mq}_{\mathrm{O}}~\underset{+}{\underset{}{+}}~\underbrace{np}_{\mathrm{I}}
\quad\quad\quad 
c=\underbrace{nq}_{\mathrm{F}}
$$

A trinomial $ax^2+bx+c$ is also called a ***quadratic polynomial***. The function defined by $f(x)=ax^2+bx+c$ is called a ***quadratic function***.

\BeginKnitrBlock{rmdtip}<div class="rmdtip">
**Trial and error.**  
The observation suggests to use trial and error to find the undetermined coefficients $m$, $n$, $p$, and $q$ from factors of $a$ and $c$ such that the sum of cross products $mq+np$ is $b$. A diagram as shown in the following examples will be helpful to check a trial.
</div>\EndKnitrBlock{rmdtip}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-25"><strong>(\#exm:unnamed-chunk-25) </strong></span>
Factor $x^2+6x+8$.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Factor $a=1$:
   $$1=1\cdot 1.$$

2. Factor $c=8$:
   $$8=1\cdot 8=2\cdot 4.$$

3. Choose a proper combination of pairs of factors and check if the sum of cross product equals $b=6$:
   $$1\cdot 4+ 1\cdot 2=6.$$  
   This step can be checked easily using the following diagram.  
   ![A picture showing the factoring of x^2+6x+8](figs/tikz-factoring-x^2+6x+8.png){width=60%}

4. Factor the trinomial
    $$x^2+6x+8=(x+2)(x+4).$$
</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-27"><strong>(\#exm:unnamed-chunk-27) </strong></span>
Factor $2x^2+5x-3$.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Factor $a=2$:
   $$1=1\cdot 2.$$

2. Factor $c=-3$:
   $$-3=1\cdot (-3)=(-1)\cdot 3.$$

3. Choose a proper combination of pairs of factors and if the sum of cross products equals $b=5$:  
   $$2\cdot 3+1\cdot(-1)=5.$$  
   This step can be checked easily using the following diagram.  
   ![A picture showing the factoring of 2x^2+5x-3](figs/tikz-factoring-2x^2+5x-3.png){width=60%}  

4. Factor the trinomial
   $$2x^2+5x-3=(x+3)(2x-1).$$
</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{rmdtip}<div class="rmdtip">
**Use Auxiliary Problem.**  
Some higher degree polynomials may be rewrite as a trinomial after a  substitution. Factoring the trinomial helps factor the polynomial.
</div>\EndKnitrBlock{rmdtip}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-30"><strong>(\#exm:unnamed-chunk-30) </strong></span>
Factor the trinomial completely.

$$4x^4-x^2-3$$
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Let $x^2=y$. Then $4x^4-x^2-3=4y^2-y-3$.

2. Factor the trinomial in $y$:   $4y^2-y-3=(4y+3)(y-1)$.

3. Replace $y$ by $x^2$ and factor further.
$$
    \begin{split}
        4x^4-x^2-3&=4y^2-y-3\\
        &=(4y+3)(y-1)\\
        &=(4x^2+3)(x^2-1)\\
        &=(4x^2+3)(x-1)(x+1).
    \end{split}
$$
</div>\EndKnitrBlock{solution}

## Practice

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-32"><strong>(\#exr:unnamed-chunk-32) </strong></span>
Factor out the GCF.

1. $18x^2y^2-12xy^3-6x^3y^4$
1. $5x(x-7)+3y(x-7)$
1. $-2a^2(x+y)+3a(x+y)$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-33"><strong>(\#exr:unnamed-chunk-33) </strong></span>
Factor by grouping.

1. $12xy-10y+18x-15$
1. $12ac-18bc-10ad+15bd$
1. $5ax-4bx-5ay+4by$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-34"><strong>(\#exr:unnamed-chunk-34) </strong></span>
Factor completely.

1. $25x^2-4$
1. $8x^3-2x$
1. $25xy^2+x$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-35"><strong>(\#exr:unnamed-chunk-35) </strong></span>
Factor completely.

1. $3x^3+6x^2-12x-24$
1. $x^4+3x^3-4x^2-12x$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-36"><strong>(\#exr:unnamed-chunk-36) </strong></span>
Factor the trinomial.

1. $x^2+4x+3$
2. $x^2+6x-7$
3. $x^2-3x-10$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-37"><strong>(\#exr:unnamed-chunk-37) </strong></span>
Factor the trinomial.

1. $5x^2+7x+2$
2. $2x^2+5x-12$
3. $3x^2-10x-8$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-38"><strong>(\#exr:unnamed-chunk-38) </strong></span>
Factor completely into polynomials with integer coefficients.

1. $x^3-5x^2+6x$
2. $4x^4-12x^2+5$
3. $2x^3y-9x^2y^2-5xy^3$
</div>\EndKnitrBlock{exercise}

<!--chapter:end:102-Factoring.Rmd-->

# Rational Expressions

## Rational Expressions

Let $p$ and $q$ be polynomial functions of $x$ and $p$ is not a constant function. We call the function $r(x)=\frac{p(x)}{q(x)}$ a \dfn{rational function}. The domain of $r$ is $\{x\mid Q(x)\neq 0\}$.
The expression $\frac{p(x)}{q(x)}$ is called a \dfn{rational expression}, the polynomial $q(x)$ \dfn{the numerator}, and the polynomial $q(x)$ \dfn{the denominator}.
A rational expression is \dfn{simplified} if the numerator and the denominator have no common factor other than $1$.

Let $p(x)$, $q(x)$ be polynomials with $q(x)\neq 0$ and $c(x)$ be a nonzero expression. Then
$$
\dfrac{~p(x)\cdot c(x)~}{~q(x)\cdot c(x)~}=\dfrac{~p(x)~}{~q(x)~}.
$$

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-39"><strong>(\#exm:unnamed-chunk-39) </strong></span>
Simplify $\dfrac{x^2+4x+3}{x^2+3x+2}$.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Factor both the top and the bottom.
$$
    \dfrac{x^2+4x+3}{x^2+3x+2}=\dfrac{(x+1)(x+3)}{(x+1)(x+2)}.
$$

1. Divide out common factors.
$$
    \dfrac{(x+1)(x+3)}{(x+1)(x+2)}=\dfrac{x+3}{x+2}.
$$
</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-41"><strong>(\#exm:unnamed-chunk-41) </strong></span>
Simplify $\dfrac{2x^2-x-3}{2x^2-3x-5}$.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Factor both the top and the bottom.
$$\dfrac{2x^2-x-3}{2x^2-3x-5}=\dfrac{(x+1)(2x-3)}{(x+1)(2x-5)}.$$

1. Divide out common factors.
$$\dfrac{(x+1)(2x-3)}{(x+1)(2x-5)}=\dfrac{2x-3}{2x-5}.$$
</div>\EndKnitrBlock{solution}

## Multiplying Rational Expressions

If $p$, $q$, $s$, $t$ are polynomials with $q\neq 0$ and $t\neq 0$, then
$$
\dfrac{~p~}{~q~}\cdot\dfrac{~s~}{~t~}=\dfrac{~ps~}{~qt~}.
$$

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-43"><strong>(\#exm:unnamed-chunk-43) </strong></span>
Multiply and then simplify.
$$\dfrac{3x^2}{x^2+x-6}\cdot\dfrac{x^2-4}{6x}.$$
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Factor numerators and denominators.
$$
    \dfrac{3x^2}{x^2+x-6}\cdot\dfrac{x^2-4}{6x}=\dfrac{3\cdot x\cdot x}{(x-2)(x+3)}\cdot\dfrac{(x-2)(x+2)}{2\cdot3\cdot x}
$$

1. Multiply and simplify.
$$
    \dfrac{\cancel{3}\cdot \cancel{x}\cdot x\cdot\cancel{(x-2)}(x+2)}{\cancel{(x-2)}(x+3)\cdot 2\cdot\cancel{3}\cdot \cancel{x}}=\dfrac{x(x+2)}{2(x+3)}
$$
</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-45"><strong>(\#exm:unnamed-chunk-45) </strong></span>
Multiply and then simplify.
$$
\dfrac{3x^2-8x-3}{x^2+8x+16}\cdot\dfrac{x^2-16}{5x^2-14x-3}.
$$
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
$$
\dfrac{3x^2-8x-3}{x^2+8x+16}\cdot\dfrac{x^2-16}{5x^2-14x-3}
=\dfrac{(3x+1)\cancel{(x-3)}\cancel{(x+4)}(x-4)}{\cancel{(x+4)}(x+4)(5x+1)\cancel{(x-3)}}
=\dfrac{(3x+1)(x-4)}{(x+4)(5x+1)}
$$
</div>\EndKnitrBlock{solution}

## Dividing Rational Expressions

If $p$, $q$, $s$, $t$ are polynomials where $q\neq 0$, $s\neq $ and $t\neq 0$, then
$$
\dfrac{~p~}{~q~}\div\dfrac{~s~}{~t~}=\dfrac{~p~}{~q~}\cdot\dfrac{~t~}{~s~}=\dfrac{~pt~}{~qs~}.
$$

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-47"><strong>(\#exm:unnamed-chunk-47) </strong></span>
Divide and then simplify.
$$
\dfrac{2x+6}{x^2-6x-7}\div \dfrac{6x-2}{2x^2-x-3}.
$$
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
1. Rewrite as a multiplication.
$$
\dfrac{2x+6}{x^2-6x-7}\div \dfrac{6x-2}{2x^2-x-3}=\dfrac{2x+6}{x^2-6x-7}\cdot \dfrac{2x^2-x-3}{6x-2}
$$

1. Factor and simplify.
$$
\dfrac{2x+6}{x^2-6x-7}\cdot\dfrac{2x^2-x-3}{6x-2}
=\dfrac{\cancel{2}(x+3)\cancel{(x+1)}(2x-3)}{\cancel{2}\cancel{(x+1)}(x-7)(3x-1)}
=\dfrac{(x+3)(2x-3)}{(x-7)(3x-1)}
$$
</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-49"><strong>(\#exr:unnamed-chunk-49) </strong></span>
Simplify.  

1. $\dfrac{3x^2-x-4}{x+1}$

2. $\dfrac{2x^2-x-3}{2x^2+3x+1}$

3. $\dfrac{x^2-9}{3x^2-8x-3}$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-50"><strong>(\#exr:unnamed-chunk-50) </strong></span>
Multiply and simplify.  

1. $\dfrac{x+5}{x+4}\cdot\dfrac{x^2+3x-4}{x^2-25}$

1. $\dfrac{3x^2-2x}{x+2}\cdot\dfrac{3x^2-4x-4}{9x^2-4}$

1. $\dfrac{6y-2}{3-y}\cdot\dfrac{y^2-6y+9}{3y^2-y}$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-51"><strong>(\#exr:unnamed-chunk-51) </strong></span>
Divide and simplify.  

1. $\dfrac{9x^2-49}{6}\div\dfrac{3x^2-x-14}{2x+4}$

2. $\dfrac{x^2+3x-10}{2x-2}\div\dfrac{x^2-5x+6}{x^2-4x+3}$

3. $\dfrac{y-x}{xy}\div\dfrac{x^2-y^2}{y^2}$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-52"><strong>(\#exr:unnamed-chunk-52) </strong></span>
Simplify.
$$
\frac{-x^2+11x-18}{x^2-4x+4}\div \frac{x^2-5x-36}{x^2-7x+12}\cdot \frac{2x^2+7x-4}{x^2+2x-15}
$$
</div>\EndKnitrBlock{exercise}

<!--chapter:end:103-Rational-Expressions.Rmd-->

# Radicals and Rational Exponents

<!--chapter:end:104-Radicals-Rational-Exponents.Rmd-->

# (PART\*) Part 2: Equations and Applications {-}

# Solve Polynomial Equations by Factoring

## Zero-Product Rule

<!--chapter:end:201-Solve-by-Factoring.Rmd-->

# Quadratic Formula

<!--chapter:end:202-Quadratic-Formula.Rmd-->

# Applications of Quadratic Equations

<!--chapter:end:203-Applications-Quadratic-Equations.Rmd-->

# Linear Inequalities

## Know the Grade You Must Earn

\BeginKnitrBlock{rmdthink}<div class="rmdthink">A course has three types of assessments: homework, monthly test and the final exam. The grading policy of the course says that homework counts 20%, monthly test counts 45% and the final exam counts for 35%. At the last day of class a student wants to know the minimum grade needed on the final to get a grade C or better, equivalently, overall grade 74 or above. The student earned 100 on homework and 80 on monthly test.

1. What the minimum grade the student must earn on the final to get a C or better?
2. If, in addition, the final exam must be at least 55 to earn a C or better, what would be the minimum grade needed?
</div>\EndKnitrBlock{rmdthink}

\begin{rmdthink}
The college student has attempted 30 credits and a cumulated GPA 1.8. To
graduate from the college, the GPA must be 2.0 or higher and the total
credits must be at least 60. Now the student decides to spend more time
on studying and aims at an cumulated GPA 2.5 on further courses.\\
How many more attempted credits the student must earn to graduate?

\textbf{Cumulated GPA =
\(\dfrac{\text{Total Quality Points Earned}}{\text{Total Attempted Credits}}\)}

\textbf{Total Quality Points Earned = Sum of
\(\text{Credits Attempted}\times \text{Grade Value}\)}
\end{rmdthink}

## Properties and Definitions

### Properties of Inequalities {-}

An inequality defines a relationship between two expressions. The following properties show when the inequality relationship is preserved or reversed.

|Property| Example |
|:---|:---|
|**The additive property** <br/>  If $a<b$, then $a+c<b+c$, for any real number $c$. <br/> If $a<b$, then $a-c<b-c$,  for any real number $c$. |If $x+3<5$, then $x+3-3<5-3$. <br/> Simplifying both sides, we get $x<2$.|
|**The positive multiplication property**  <br/> If $a<b$ and $c$ is positive, then $ac<bc$. <br/>   If $a<b$ and $c$ is positive, then $\frac ac<\frac bc$. |If $2x<4$, then $\frac{2x}{2}<\frac{4}{2}$. <br/>  Simplifying both sides, we get $x<2$.|
|**The negative multiplication property**  <br/> If $a<b$ and $c$ is negative, then $ac>bc$.  <br/>  If $a<b$ and $c$ is negative, then $\frac ac>\frac bc$. |If $1<2$, then $-2=1\cdot(-2)>2\cdot(-2)=-4$. <br/>  If $-2x<4$, then $\frac{-2x}{-2}>\frac{4}{-2}$.  <br/>  Simplifying both sides, we get $x>2$.|

\BeginKnitrBlock{rmdnote}<div class="rmdnote">These properties also apply to $a\leq b$, $a>b$ and $a\geq b$.</div>\EndKnitrBlock{rmdnote}

\BeginKnitrBlock{rmdnote}<div class="rmdnote">It's always better to view $a-c$ as $a+(-c)$. Because addition has the commutative property.</div>\EndKnitrBlock{rmdnote}

### Compound Inequalities {-}

A ***compound inequality*** is formed by two inequalities with the word  *and* or the word *or*. For examples, the following are three commonly seen type compound inequalities:
$$
x-1>2\quad \text{and} \quad 2x+1<3,
$$
$$
3x-5<4\quad \text{or} \quad 3x-2>10,
$$
$$
-3\leq \frac{2x-4}{3}<2.
$$
The third compound inequality is simplified expression for the compound inequality $-3\leq \frac{2x-4}{3}$ and $\frac{2x-4}{3}<2$.

### Interval Notations {-}

Solutions to an inequality normally form an interval which has boundaries and should reflect inequality signs. Depending on the form of  an inequality, we may a single interval and a union of intervals. For example, suppose $a<b$, we have the following equivalent representations of inequalities.

| $x<a$ |$x\ge b$ |$a\le x<b$ |$x\le a$ or $x>b$ |
|:---:|:---:|:---:|:---:|
| ![less than](figs/Interval-number-line-less-than.png){max-width=10%} | ![greater than](figs/Interval-number-line-greater-than.png){max-width=10%} |![between](figs/Interval-number-line-between.png){max-width=10%} | ![beyond](figs/Interval-number-line-beyond.png){max-width=10%}|
|$(-\infty, a)$|$[b,\infty)$|$[a, b)$|$(-\infty, a]\cup (b,\infty)$|

## Examples

\BeginKnitrBlock{rmdtip}<div class="rmdtip">**Think backward.** To solve a problem, knowing what to expect helps you narrow down the gap step by step by comparing the goal and your achievement.

An inequality (equation) is solved if the unknown variable is isolated. That's what to be expected. To isolate the unknown variable, you use comparisons to determine what mathematical operations should be applied. When an operation is applied to one side, the same operation should also be applied to the other side. For inequalities, we also need to determine whether the inequality sign should be preserved or reversed according to the operation.</div>\EndKnitrBlock{rmdtip}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-58"><strong>(\#exm:unnamed-chunk-58) </strong></span>Solve the linear inequality
$$
2x+4>0.
$$</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}$$
\begin{aligned}
&  & 2x+4 & >0  \\
    \text{add $-4$}      &  & 2x   & >-4 \\
    \text{divide by $2$} &  & x    & >-2
\end{aligned}
$$
The solution set is $(-2, \infty)$.</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-60"><strong>(\#exm:unnamed-chunk-60) </strong></span>Solve the linear inequality 
$$
-3x-4<2.
$$</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}$$
\begin{aligned}
                                        &  & -3x-4 & <2       \\
    \text{add $4$}                   &  & -3x   & <6  &  & \\
    \text{divide by $-3$ and switch} &  & x     & >-2
\end{aligned}
$$
The solution set is $(-2, +\infty)$.</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-62"><strong>(\#exm:unnamed-chunk-62) </strong></span>Solve the compound linear inequality 
$$
x+2<3\quad \text{and}\quad -2x-3<1.
$$</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}$$
\begin{aligned}
    x+2 & <3 &  & \text{and} & -2x-3 & <1  \\
    x   & <1 &  &            & -2x   & <4  \\
    x   & <1 &  & \text{and} & x     & >-2
\end{aligned}
$$
That is $-2<x<1$. The solution set is $(-2, 1)$.</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-64"><strong>(\#exm:unnamed-chunk-64) </strong></span>Solve the compound linear inequality  
$$
-x+4>2 \quad \text{or} \quad 2x-5\geq -3.
$$</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}$$
\begin{aligned}
    -x+4 & >2  &  & \text{or} & 2x-5 & \geq -3 \\
    -x   & >-2 &  &           & 2x   & \geq 2  \\
    x    & <2  &  & \text{or} & x    & \geq 1
\end{aligned}
$$
That is $x\geq 1$ or $x< 2$. The solution set is $(-\infty, +\infty)$.</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-66"><strong>(\#exm:unnamed-chunk-66) </strong></span>Solve the compound linear inequality
$$
-4\leq\dfrac{2x-4}{3}<2.
$$</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}$$
\begin{array}{rcl}
    -4\leq  & \dfrac{2x-4}{3}    & <2  \\
    -12\leq & 2x-4         & <6  \\
    -8\leq  & 2x                & <10 \\
    -4\leq  & x               & <5  
\end{array}
$$
The solution set is $[-4, 5)$.</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-68"><strong>(\#exm:unnamed-chunk-68) </strong></span>Solve the compound linear inequality
$$
-1\leq \dfrac{-3x+4}{2}<3.
$$</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}$$
\begin{array}{rcl}
    -1\leq & \frac{-3x+4}{2}  & <3        \\
    -2\leq & -3x+4          & <6        \\
    -6\leq & -3x           & <2        \\
    2\geq  & x            & >-\frac23
\end{array}
$$
The solution set is $(-\frac23, 2]$.</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{example}<div class="example"><span class="example" id="exm:unnamed-chunk-70"><strong>(\#exm:unnamed-chunk-70) </strong></span>
Suppose that $-1\le x < 2$. Find the range of $5-3x$. Write your answer in interval notation.
</div>\EndKnitrBlock{example}

\BeginKnitrBlock{solution}<div class="solution">\iffalse{} <span class="solution"><em>Solution. </em></span>  \fi{}
To get $5-3x$ from $x$, we need first multiply $x$ be $-3$ and then add $5$.
$$
\begin{array}{rcl}
-1\leq & x          & < 2        \\
3\geq & -3x         & >-6        \\
8\geq & 5-3x      & >-1
\end{array}
$$
The range of $5-3x$ is $(-1, 8]$.
</div>\EndKnitrBlock{solution}

\BeginKnitrBlock{rmdtip}<div class="rmdtip">
**Understand the Problem.** Understanding the known, the unknown and the condition of the given problem is the key to solve the problem. Normally, by comparing the known and unknown, you will find the way to solve the problem.
</div>\EndKnitrBlock{rmdtip}

## Practice

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-73"><strong>(\#exr:unnamed-chunk-73) </strong></span>
Solve the linear inequality. **Write your answer in interval notation.**

1. $3x + 7 \leq 1$
2. $2x-3>1$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-74"><strong>(\#exr:unnamed-chunk-74) </strong></span>
Solve the linear inequality. **Write your answer in interval notation.**

1. $4x + 7 > 2x-3$
2. $3-2x \le x-6$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-75"><strong>(\#exr:unnamed-chunk-75) </strong></span>
Solve the compound linear inequality. **Write your answer in interval notation.**

1. $3x+2>-1 ~\text{and}~ 2x-7\leq 1$
2. $4x -7< 5 ~\text{and}~ 5x-2\geq 3$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-76"><strong>(\#exr:unnamed-chunk-76) </strong></span>
Solve the compound linear inequality. **Write your answer in interval notation.**

1.  $-4\leq 3x+5<11$
2.  $7\geq 2x-3\geq -7$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-77"><strong>(\#exr:unnamed-chunk-77) </strong></span>
Solve the compound linear inequality. **Write your answer in interval notation.**

<div class="row">
1.  $3x-5>-2 ~\text{or}~ 10-2x\leq 4$
2.  $2x + 7<5 ~\text{or}~ 3x-8\geq x-2$
</div>

</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-78"><strong>(\#exr:unnamed-chunk-78) </strong></span>
Solve the compound linear inequality. **Write your answer in interval notation.**

1.  $-2\leq \dfrac{2x-5}{3}<3$
1.  $-1< \dfrac{3x+7}{2}\leq 4$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-79"><strong>(\#exr:unnamed-chunk-79) </strong></span>
Solve the linear inequality. **Write your answer in interval notation.**
$$
\frac13x+1<\frac12(2x-3)-1
$$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-80"><strong>(\#exr:unnamed-chunk-80) </strong></span>
Solve the compound linear inequality. **Write your answer in interval notation.**
$$
0\le \frac25-\frac{x+1}{3}< 1
$$
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-81"><strong>(\#exr:unnamed-chunk-81) </strong></span>
Suppose $0< x \le 1$. Find the range of $-2x+1$. **Write your answer in interval notation.**
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-82"><strong>(\#exr:unnamed-chunk-82) </strong></span>
Suppose that $x+2y=1$ and $1\leq x< 3$. Find the range of $y$. **Write your answer in interval notation.**
</div>\EndKnitrBlock{exercise}

\BeginKnitrBlock{exercise}<div class="exercise"><span class="exercise" id="exr:unnamed-chunk-83"><strong>(\#exr:unnamed-chunk-83) </strong></span>
A toy store has a promotion “Buy one get the second one half price" on a certain popular toy. The sale price of the toy is \$20 each. Suppose the store makes more profit when you buy two. What do you think the store's purchasing price of the toy is?
</div>\EndKnitrBlock{exercise}

<!--chapter:end:204-Linear-Inequalities.Rmd-->

# (PART\*) Part 3: Functions and Applications {-}

# Introduction to Functions

## Sets, Order Pairs, and the Rectangular Coordinate System

## Functions Defined by Equations

## Graphs of Functions

<!--chapter:end:301-Introduction-to-functions.Rmd-->

# Linear Functions

<!--chapter:end:302-Linear-functions.Rmd-->

# Quadratic Functions

## The Complete Square Form

<!--chapter:end:303-Quadratic-functions.Rmd-->

# Rational and Radical Functions

<!--chapter:end:304-Rational-Radical-functions.Rmd-->

# Exponential Functions

<!--chapter:end:305-Exp-functions.Rmd-->

# Logarithmic Functions

<!--chapter:end:306-Log-functions.Rmd-->

# Applications of Exponential and Logarithmic Functions

## Exponential Equations

## Logarithmic Equations

## Applications

<!--chapter:end:307-Exp-Log-Equations.Rmd-->
