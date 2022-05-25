<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script> 

$$\newcommand{\dv}[1]{  \frac{\textrm{d}}{\textrm{d}#1}  }$$
$$\newcommand{\de}{\textrm{d}} $$
$$\newcommand{\gr}[1]{\textbf{#1}} $$


https://gattock.github.io/jelly-book.github.io/

--HOW TO SET WIDTH FULL PAGE? --

## Vector fields general info
We consider a vector field, let´s say a bidimensional velocity field of a continuum fluid. We can express in in different notations: we can write \\

$$\mathbf{u}= \vec u= u \hat e_1 + v \hat e_2 = \begin{bmatrix} u \\ v \end{bmatrix} $$

$$\mathbf{u}= \vec u= u \hat e_1 + v \hat e_2 = \begin{bmatrix} u & v \end{bmatrix} $$

where $$ (e_1 e_2) $$ is an ortho-normal (ON) basis for the plane $$\mathbb{R}^2$$ . 

--FIRST VIDEO FLOW MOTION--

Embedding videos: 

<p align="center">
<iframe width="560" height="315" src="https://www.youtube.com/watch?v=hjMx8EuyZJ8" title="RandomTitle" frameborder="0"
allow="accelerometer; autoplay; clipboard-write; ecnrypted-media; gyroscope; picture-in-picture"
allowfullscreen></iframe>
</p>

Now we consider an arbitrary domain $$ \Omega $$ --VIDEO 2: arbitrary omegas-- 

Keeping the case of the fluid flow, we already know by conservation law that the total amount of mass must be conserved if nothing is added or removed inside the domain: 

$$ \dv{t}[ \int \rho (x,y) dx dy]=0   $$

SASA PROVA

$$ \dv{t}[ \int \rho (x,y) \de x \de y]=0   $$

We can intuitively see that the total amount of mass inside a 2D closed system (no flux through boundaries) varies by the surface integral of the source function $$f(x,y)$$ :

$$ \dv{t} \int_{\Omega} $$

This means that the temporal variation of the mass inside the domain is given by the average of the source function in the domain:
$$ \dv{t} \int_{\Omega} \rho(x,y) \de x \de y = \int_{\Omega} f(x,y) \de x \de y $$

--indicate with underbrace: total mass on rho integral, resulting inlet/outlet on f integral --

--Video: flux tangential to the boundary or approaching with 0 speed or negative source function on boundary --

If we consider a non-zero flux through boundaries it becomes:

$$ \dv{t} \int_{\Omega} \rho(x,y) \de x \de y = \int_{\Omega} f(x,y) \de x \de y - \oint_{\partial \Omega} \vec u \cdot \hat n \de l $$
where the last term is the flux integral across the domain boundary

So, we have seen that the contributes to the average density inside an arbitrary domain are given by:

* Flux, positive outward (-)
* Source function (+)

This idea can be extended for arbitrarily small domain! this leads to..... ---FINISH--

## 1D case:

Let´s consider a 1D vector field, in particular the "mass inside dl": if dl tends to zero, we can write $$ \de m= \rho \de x $$ .
For simplicity we suppose that the source function is zero everywhere: $$f(x)=0$$
The resulting variation of density is given by the difference of speed between the left boundary (a point) and the right boundary.
If $$ \de x \to 0$$ this difference will be a derivative: 

$$ \dv{t} m = \dv{t} \rho \de x = u(x+ \de x) - u(x) \Rightarrow \dv{t} \rho = \frac{u(x+ \de x) - u(x)}{\de x}= \dv{x} u(x) $$

So we see how the time variation of mass in this case is the derivative of the velocity field: in dimension higher than one this concept is generalized by the \gr{divergence}

## 2D case:

-- ATTACH VIDEO FLUX THROUGH SQUARE--
<p align="center">
<iframe width="560" height="315" src="https://www.youtube.com/watch?v=hjMx8EuyZJ8" title="RandomTitle" frameborder="0"
allow="accelerometer; autoplay; clipboard-write; ecnrypted-media; gyroscope; picture-in-picture"
allowfullscreen></iframe>
</p>

With the same fashion we compute:

$$  \dv{t} \rho = \rho \Big[  u(x,y) - u(x+ \de x,y) \Big] + \rho \Big[  v(x,y) - v(x,y+ \de y) \Big] $$ --CHECK!! $$ \rho$$ !! --

and for $$ \de x , \de y \to 0  $$ it becomes:

$$  \dv{t} \rho = - \rho \Big( \dv{x} u(x,y) + \dv{y} v(x,y) \Big) $$

## The divergence 

The last equation express the divergence of the velocity vector field $$\mathbf{u}= \vec u= u \hat e_1 + v \hat e_2 = \begin{bmatrix} u & v \end{bmatrix} $$ in 2D.

The divergence of a vector field is defined as the scalar product with the gradient operator: in 2D is defined in the following way

$$ \textrm{div} \, \vec u = \nabla \cdot \vec u =  \dv{x} u(x,y) + \dv{y} v(x,y)  $$

Indeed "unrolling" the divergence operator leads to:

$$ \nabla \cdot \vec u =  \begin{bmatrix} \dv{x} & \dv{y} \end{bmatrix} \cdot \begin{bmatrix} u & v \end{bmatrix}= \Big( \dv{x} u(x,y) + \dv{y} v(x,y) \Big)   $$




-- video divergence--

## Sink and sources

Every point in the domain can behave as "source" (+) or "sink" (-): this behavior is described by the source function $$f(x,y)$$ being positive or negative.

Please, Note: the value of the source function must not be confused with the value of the divergence! Indeed, the divergence consider only the variation of the speed field around a point, but doesn´t give information whether mass is generated(-removed) or compressed(-decompressed)! Assuming the more general case of compressible flow, also the density variation in a point is related with the divergence of the field. Let´s see this more in detail:
--video compression-decompression-with sources-- in different points different behaviors.

## Continuity equation
To keep track of the contributions of both the source function and the behavior of neighbor fluid particles, we have just to sum up those, and this leads to the \gr{continuity equation}.

$$  \dv{t} \rho(x,y) = f(x,y) -\nabla \cdot ( \rho \vec u(x,y) ) $$

In case of incompressible fluid, we know that $$ \rho=\textrm{cost.}  $$
This leads directly to
$$  \nabla \cdot ( \rho \vec u(x,y) )= f(x,y) $$
that intuitively means that the divergence of the velocity field is given only by how much fluid is "generated-absorbed" in that point.

--VIDEO WITH CHEMICALS REACTIONS AND COMPOUNDS DENSITIES VARIATIONS--




## MY STUFF

Links to chapter1: 
* https://gattock.github.io/jelly-book.github.io/chapter1/
    + https://jelly-book.github.io/2022/05/24/chapter1.html 
    + https://gattock.github.io/jelly-book.github.io/2022/05/24/chapter1.html 
        - https://gattock.github.io/jelly-book.github.io/2022/05/24/VectorFields.html


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
