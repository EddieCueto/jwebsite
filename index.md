@def hascode = true

# Welcome to my blog

<!-- \tableofcontents  you can use \toc as well -->

This blog is where I intent to update my projects as well as my research. I am doing this right now due to COVID-19 and the fact that the epidemic started when I was about to start a PhD position in TU Dublin.
Currently I've been working in two "big" projects:
* `Setting up this blog` and
* `Create complexity measures for Deep Neural Networks (DNN)`.

Both of this projects are being developed with [Julia](https://julialang.org/), language which was introduced to my during my time at Instituto Politécnico Nacional [IPN](https://www.ipn.mx/). The Julia packages that I am either using or extending are [Flux.jl](https://fluxml.ai/) and [Franklin.jl](https://franklinjl.org/).

A small snippet of Julia:
```julia
abstract type Point end
struct PointR2{T<:Real} <: Point
    x::T
    y::T
end
struct PointR3{T<:Real} <: Point
    x::T
    y::T
    z::T
end
function len(p::T) where T<:Point
  sqrt(sum(getfield(p, η)^2 for η ∈ fieldnames(T)))
end
```

## A bit about myself

My interest in science started from a very early age I was in love with physics because a teacher in elementary school had a copy of the book `COSMOS` which he lend me and I was marveled by the words of [Carl Sagan](https://en.wikipedia.org/wiki/Carl_Sagan)

<!--
# Building static websites in Julia

\blurb{Franklin is a simple, customisable static site generator oriented towards technical blogging and light, fast-loading pages.}

## Key features

@@flist
* \goto{/syntax/markdown/} Augmented markdown allowing definition of LaTeX-like commands,
* \goto{/syntax/divs-commands/} Easy inclusion of user-defined div-blocks,
* \goto{/syntax/divs-commands/} Maths rendered via [KaTeX](https://katex.org/), code via [highlight.js](https://highlightjs.org) both can be pre-rendered,
* \goto{/code/} Can live-evaluate Julia code blocks,
* \goto{/workflow/#creating_your_website} Live preview of modifications,
* \goto{/workflow/#optimisation_step} Simple optimisation step to compress and pre-render the website,
* \goto{/workflow/#publication_step} Simple publication step to deploy the website,
* \goto{/code/literate/} Straightforward integration with [Literate.jl](https://github.com/fredrikekre/Literate.jl).
@@

## Quick start

To install Franklin with Julia **≥ 1.3**,

```julia-repl
(v1.4) pkg> add Franklin
```

You can then just try it out:

```julia-repl
julia> using Franklin
julia> newsite("mySite", template="pure-sm")
✓ Website folder generated at "mySite" (now the current directory).
→ Use serve() from Franklin to see the website in your browser.

julia> serve()
→ Initial full pass...
→ Starting the server...
✓ LiveServer listening on http://localhost:8000/ ...
  (use CTRL+C to shut down)
```

If you navigate to that URL in your browser, you will see the website. If you then open `index.md` in an  editor and modify it at will, the changes will be live rendered in your browser.
You can also inspect the file `menu1.md` which offers more examples of what Franklin can do.

## Installing optional extras

Franklin allows a post-processing step to compress HTML and CSS and pre-render code blocks and math environments.
This requires a couple of dependencies:
@@tlist
* [`python3`](https://www.python.org/downloads/) for the minification of the site,
* [`node.js`](https://nodejs.org/en/) for the pre-rendering of KaTeX and code highlighting.
@@
You will then need to install `highlight.js`, which you should do from Julia using the [NodeJS.jl](https://github.com/davidanthoff/NodeJS.jl) package:

```julia-repl
julia> using NodeJS
julia> run(`sudo $(npm_cmd()) install highlight.js`)
```

**Note**: a key advantage of using `NodeJS` for this instead of using `npm` yourself is that it puts the libraries in the "right place" for Julia to find them.

Assuming you have `python3`, Franklin will try to install the python package [`css_html_js_minify`](https://github.com/juancarlospaco/css-html-js-minify) if via `pip3`.
-->