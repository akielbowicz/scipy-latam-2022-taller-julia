---
theme : "solarized"
transition: "slide"
highlightTheme: "monokai"
logoImg: "https://pythoncientifico.ar/static/assets/images/scipy-la-2022_logo-header.svg"
slideNumber: false
title: "Julia para Pythonistas"
---

# Taller de Julia ✨ para Pythonistas 🐍

SciPy Latam 2022, Salta, Argentina.

Miercoles 28 de Septiembre, 2022
---

> ¿Qué viene antes de Julia?

<span class="fragment">> Augusto </span>
<span class="fragment">**Sasha** </span>
<span class="fragment">Kielbowicz</span>

--

> Augusto **Sasha** Kielbowicz

Originario de

![🇪🇨 :ecuador:](https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/240/joypixels/340/flag-ecuador_1f1ea-1f1e8.png)

--

> Augusto **Sasha** Kielbowicz

Criado en Quito y Catamarca

![🇪🇨 :ecuador:](https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/240/joypixels/340/flag-ecuador_1f1ea-1f1e8.png)
![🇦🇷 :argentina:](https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/240/joypixels/340/flag-argentina_1f1e6-1f1f7.png)

--

> Augusto **Sasha** Kielbowicz

- Estudié Física en la UBA 👨‍🔬⚛️ {.fragment }
- Programador autodidacta 🐍 🧮 📚 {.fragment }
- Trabajo como `Quantitative Developer` 👨‍💻 📈📉💸 {.fragment}

![logo-qontigo](https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/Qontigo-v1_subs_block_rgb.png/320px-Qontigo-v1_subs_block_rgb.png) {.fragment .fade-in-then-out}

🤓 {.fragment .fade-in}

---

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

--

![qr](data:image/gif;base64,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)

[https://github.com/akielbowicz/scipy-latam-2022-taller-julia/](https://github.com/akielbowicz/scipy-latam-2022-taller-julia/tree/main)

---

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

> We want a language that's open source, with a liberal license.

---

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

> Queremos un lenguaje que sea de `codigo abierto`,
con una licencia liberal.

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

> We want the speed of C with the dynamism of Ruby.

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

> Queremos la velocidad de `C` con el dinamismo
de `Ruby`.

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

> We want a language that's homoiconic, with true macros like Lisp, but with obvious, familiar mathematical notation like Matlab.

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

> Queremos un lenguaje que sea `homoiconico`,

--

<!-- .slide: data-background="https://media2.giphy.com/media/WGvwSV5qjBJuYPbzcT/giphy.gif?cid=ecf05e47fvlsllqsek3m6y4tuohs5uv5oonqc38nuztgrvl0&rid=giphy.gif&ct=g" -->

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

> Queremos un lenguaje que sea `homoiconico`,
<span class="fragment">con *macros* verdaderos como `Lisp`,</span>
<span class="fragment">pero con la familiar notacion matematatica como
`Matlab`</span>

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

> We want something as usable for general programming as Python, as easy for statistics as R, as natural for string processing as Perl, as powerful for linear algebra as Matlab, as good at gluing programs together as the shell.

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

> Queremos que sea utilizable para programacion
general como 
<span class="fragment">`Python`,</span>
<span class="fragment">tan facil para la estadistica como </span>
<span class="fragment">`R`,</span>
<span class="fragment">tan natural para procesamiento de texto como </span>
<span class="fragment">`Perl`,</span>
<span class="fragment">tan poderoso para *algebra lineal* como </span>
<span class="fragment">`Matlab`,</span>
<span class="fragment">tan bueno en unir programas como la </span>
<span class="fragment">`shell`.</span>

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

>Something that is dirt simple to learn, yet keeps the most serious hackers happy.

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

>Algo que sea muy simple para aprender,
 pero que deje feliz a los *hackers* mas solemnes

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

>We want it interactive and we want it compiled.

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

>Lo queremos **interactivo**
<span class="fragment"> y lo queremos **compilado**.</span>

--

![julia-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Julia_Programming_Language_Logo.svg/320px-Julia_Programming_Language_Logo.svg.png)

[Why we created julia](https://julialang.org/blog/2012/02/why-we-created-julia/)

--

![matlab-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/2/21/Matlab_Logo.png/267px-Matlab_Logo.png)
![scipy-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b2/SCIPY_2.svg/240px-SCIPY_2.svg.png)

![wolfram-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/2/20/Mathematica_Logo.svg/230px-Mathematica_Logo.svg.png)
![octave-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/Gnu-octave-logo.svg/240px-Gnu-octave-logo.svg.png)
![r-logo](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/R_logo.svg/310px-R_logo.svg.png)

---

## **Hora de Codear**

<!-- .slide: data-background="https://media4.giphy.com/media/PI3QGKFN6XZUCMMqJm/giphy.gif?cid=ecf05e47cj84xy2o9r8p2ve9k1y9m7cen7wnz0r7dwset9ns&rid=giphy.gif&ct=g" -->

---

## Paquetes

[JuliaHub](https://juliahub.com/ui/Packages)

---

## Materiales adicionales

--

### Redes

- [JuliaLang Argentina](https://t.me/julialangarg) Telegram
- [Discourse](https://discourse.julialang.org/)
- [Zulip](https://julialang.zulipchat.com/)
- [Slack](https://julialang.slack.com/)
- [Humas of Julia](https://discord.com/invite/nPPZy4RYbP) Discord

--

### Foros

- [Forem](https://forem.julialang.org/)
- [Julia Bloggers](https://www.juliabloggers.com/) (agregador de posts)

--

### Libros

- [Hands-On Design Patterns and Best Practices with Julia](https://www.packtpub.com/product/hands-on-design-patterns-and-best-practices-with-julia/9781838648817)
- [Julia High Performance](https://www.packtpub.com/product/julia-1-0-high-performance/9781788298117)
- [Data Science in Julia for Hackers](https://datasciencejuliahackers.com/) (digital y libre)
- [Think Julia](https://www.oreilly.com/library/view/think-julia/9781492045021/)
- [Muuuchos libros más...](https://julialang.org/learning/books/)

--

### Cursos

- Curso [MIT Computational Thinking](https://computationalthinking.mit.edu/Spring21/)
- Curso [Parallel Computing and Scientific Machine Learning (SciML): Methods and Applications](https://book.sciml.ai/)

--

### Videos

- El canal de YouTube [The Julia Programming Language](https://www.youtube.com/c/TheJuliaLanguage)
- El canal de [doggo dot jl](https://www.youtube.com/c/juliafortalentedamateurs/playlists) (julia for talented amateurs)
