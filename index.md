@def title = "Franklin Sandbox"
@def hasmath = true
@def hascode = true


# Set up

## Update title

## Update config.md file

* change author

* add site name for GitHub

## Create a table of contents (optional)

\toc

## Upload using GitHub Desktop

# Examples

## How to enter text

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse posuere quis ante et placerat. Cras vitae massa sed nisl feugiat molestie. Morbi lobortis aliquam tempus. Aenean tincidunt mattis quam id lacinia. Proin sagittis, nisi at fermentum interdum, libero nunc facilisis lacus, vitae consectetur magna arcu a dolor. Curabitur dignissim a tellus ut eleifend. Ut vestibulum risus non ultrices sodales. Cras in pretium arcu, eget tristique ex. Maecenas ultrices auctor enim nec imperdiet.

Aliquam sollicitudin vulputate eros, semper vulputate ante. Curabitur euismod, mauris a semper maximus, risus mi venenatis enim, et finibus neque metus vel enim. Phasellus eget sagittis tellus, nec vulputate tellus. Aenean laoreet nibh quis orci suscipit lacinia. Donec ac magna enim. In augue nunc, pulvinar dignissim consectetur non, vehicula quis nulla. Etiam tempus quis risus id posuere. Maecenas maximus velit in ultrices viverra. Aliquam in felis ac dolor imperdiet suscipit. Phasellus posuere nunc cursus, mollis tortor id, luctus neque. Nulla ornare, massa in tempor rutrum, nibh sem cursus lacus, id euismod nunc ante nec diam. Praesent vitae venenatis nulla.

## How to render math equations

$$  x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a} $$

$$ \tan A = \frac{\sin A}{\cos A}  $$

$$ \lim_{h \to 0} \frac{f(x+h) - f(x)}{h} $$

$$ \int_a^b f(x) dx = F(b) - F(a) $$

$$ \frac{d}{dx} \int_a^x f(t)dt = f(x) $$

$$  \sum \mathbf{F} = 0 \Leftrightarrow \frac{d\mathbf{v}}{dt} = 0 \\
    \bold{F} = m\bold{a} \\
    \bold{F}_A = - \bold{F}_B
$$

$$  \bar x = \frac 1n \bigg( \sum_{i=1}^n x_i \bigg) = \frac{x_1 + x_2 + \dots + x_n}{n} 
$$

## How to insert Julia code (with outputs!)

```julia:./ex11
println("Hello, World!")
```

\show{./ex11}

Basic Math

```julia:./ex12
1 + 1
```

\show{./ex12}

Create function

```julia:./ex13
function add(x, y)
    x + y
end
```

\show{./ex13}

Call function

```julia:./ex14
add(2, 3)
```

\show{./ex14}

Random numbers

```julia:./ex15
rand(5, 5)
```

\show{./ex15}

## How to insert a table from a CSV file

World Population by Region by Year:

\tableinput{}{./tableinput/population_by_year.csv}

@@source
Source: Wikipedia
@@

## How to insert and image file

![beeswarm plot of population by region](/assets/p_beeswarm_region.svg)

@@source
Source: Wikipedia
@@

## How to insert a clickable thumbnail to a Youtube video

[![YT thumbnail](https://img.youtube.com/vi/AilZwXgglsI/0.jpg)](https://youtu.be/AilZwXgglsI)

## How to inject raw HTML

~~~
<iframe width="640" height="396" src="https://www.youtube.com/embed/fVBiLEtZB7A" title="[03x09] Intro to Franklin, a Julia Static Site Generator | 9/13 | Julia Web Tools for Beginners" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
~~~

<!--
# Franklin syntax sandbox

This page is meant as a sandbox for Franklin Syntax so that you can quickly practice or experience things.

## Sandbox

Write whatever you want here to practice Franklin Syntax:

```julia:./ex1
using LinearAlgebra, Random
Random.seed!(135)
a, b = randn(50), randn(50)
println(dot(a, b))
println(sum(ai * bi for (ai, bi) ∈ zip(a, b)))
```

\output{./ex1}

(yet another example that floating point arithmetics can be complicated).

$$ \forall x \in \R:\quad \scal{x, x} \ge 0 $$

\newcommand{\E}{\mathbb E}

Surely some people remember the ordering, but I always forget:

$$ \varphi(\E[X]) \le \E[\varphi(X)] $$

for $\varphi$ convex.
-->