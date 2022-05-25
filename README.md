<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script> 

\newcommand{\dv}[1][2]{  \frac{\textrm{d}#1}{\textrm{d}#1}  }
\newcommand{\de}{\textrm{d}}
$$\newcommand{\de}{\textrm{d}} $$


https://gattock.github.io/jelly-book.github.io/
## Vector fields general info
We consider a vector field, let´s say a bidimensional velocity field of a continuum fluid. We can express in in different notations: we can write \\

$$\mathbf{u}= \vec u= u \hat e_1 + v \hat e_2 = \begin{bmatrix} u \\ v \end{bmatrix} $$

$$\mathbf{u}= \vec u= u \hat e_1 + v \hat e_2 = \begin{bmatrix} u & v \end{bmatrix} $$

where $$ (e_1 e_2) $$ is an ortho-normal (ON) basis for the plane $$\mathbb{R}^2$$ . 

--FIRST VIDEO FLOW MOTION--

Now we consider an arbitrary domain $$ \Omega $$ --VIDEO 2: arbitrary omegas-- 

Keeping the case of the fluid flow, we already know by conservation law that the total amount of mass must be conserved if nothing is added or removed inside the domain: 

$$ \frac{\textrm{d}}{\textrm{d}t}[ \int \rho (x,y) dx dy]=0   $$

SASA PROVA

$$ \dv{}{t}[ \int \rho (x,y) dx dy]=0   $$

We can intuitively see that the total amount of mass inside a 2D closed system (no flux through boundaries) varies by the surface integral of the source function $$f(x,y)$$ :

$$ \frac{\de}{\de t} \int_{\Omega} $$

hola 

$$ \frac{\de{}}{\de{} t} \int_{\Omega} $$





## The divergence 



-- video divergence--

## Sink and sources

Also, every point can behave as "source" (+) or "sink" (-): this behavior is described by the source function $$f(x,y)$$ being positive or negative.

Please, Note: the value of the source function must not be confused with the value of the divergence: indeed the divergence consider only the variation of the speed field around a point, but doesn´t give information whether mass is generated or removed! Indeed, assuming the more general case of compressible flow, also the density variation in a point is related with the divergence of the field. Let´s see this more in detail:
--video compression-decompression--



## Embedding videos 

<p align="center">
<iframe width="560" height="315" src="https://www.youtube.com/watch?v=hjMx8EuyZJ8" title="RandomTitle" frameborder="0"
allow="accelerometer; autoplay; clipboard-write; ecnrypted-media; gyroscope; picture-in-picture"
allowfullscreen></iframe>
</p>


## MY STUFF

Links to chapter1: 
https://gattock.github.io/jelly-book.github.io/chapter1/
https://jelly-book.github.io/2022/05/24/chapter1.html
https://gattock.github.io/jelly-book.github.io/2022/05/24/chapter1.html
https://gattock.github.io/jelly-book.github.io/2022/05/24/VectorFields.html

Esempio 1
$e^{i \pi} = -1$

Esempio2
<img src="https://latex.codecogs.com/svg.latex?\Large&space;x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}" title="\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}" />

Esempio3
h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x

Esempio4
![\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}](https://latex.codecogs.com/svg.latex?\Large&space;x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}) 

Esempio5
$$\begin{bmatrix}1 & x_{1}\\
1 & x_{2}\\
1 & x_{3}
\end{bmatrix}$$

Esempio6
$$\mathbf{u} = 5\vec u+7\hat y$$




## Embedding LateX

```{=latex}
\begin{tabular}{ll}
A & B \\
A & B \\
\end{tabular}
```



## Welcome to GitHub Pages

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/gattock/didactic-guacamole.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
