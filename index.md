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
