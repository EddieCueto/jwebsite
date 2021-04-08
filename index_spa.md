
@def hascode = true

# Bienvenido a mi Blog

<!-- \tableofcontents  you can use \toc as well -->

Este blog es donde pretendo dar actualizaciones de mis proyectos y mi trabajo de investigación. He comenzado este blog debido al COVID-19 ya que la pandemia comenzó unos días antes de que realizara mi viaje a la ciudad de Dublín a comenzar mi doctorado. 
Actualmente trabajo en dos proyectos "grandes":
* `Actualizar este Blog` and `traducirlo al español`
* `Implementar métodos de compresión para los Modelos de Redes Neuronales Profundas`.

Ambos proyectos se están implementado en el lenguaje de programación [Julia](https://julialang.org/), el cual fue presentado por primera vez durante la maestría en el Centro de Investigación en Computación del IPN [CIC-IPN](https://www.cic.ipn.mx/index.php/es/). Los paquetes que estoy utilizando o extendiendo para este fin són 
Both of this projects are being developed with [Julia](), language which was introduced to my during my time at Instituto Politécnico Nacional. The Julia packages that I am either using or extending are [Flux.jl](https://fluxml.ai/) and [Franklin.jl](https://franklinjl.org/).

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

My interest in science started from a very early age I was in love with physics because a teacher in elementary school had a copy of the book `COSMOS` which he lend me and I was marveled by the words of [Carl Sagan](https://en.wikipedia.org/wiki/Carl_Sagan). A few years later I discovered chemistry and gave it a try but found it a bit expensive and hard so I kept trying to find "my calling", until as a teenager I got my first PC thanks to working in tending yards and some money that my parents were able to lend me.

It was an old HP machine that had installed Windows Me  ha,ha,ha one of the first things that I did was to open it to see how it was inside. After a few week, while browsing the web I read that there was something known as programming that allowed people to do stuff on computers, so a first attempt to learn to program was done in Basic and failed. In the following years due to some economical problems in my family I had to postpone my education for a few years, but was able to resume.

After my "sabbatical" I was able to finish a bachelor in mathematics which I loved, yes after some years I was able to find my calling and learned to program in C++ (which I don't use any more :P). But some of the biggest questions that I still have were not answered during my time in university. Mostly what is computation and why are there some problems harder to solve than others (some are even impossible to solve). So, as the very naive and curious person that I am, started a master in computer science and it was the best time of my life, living in one of the biggest cities of the world and working in one of the best research centers in Mexico [CIC-IPN](http://www.cic.ipn.mx/index.php/es/).

Finally in this last years I got a position as a lead data analyst on a machine learning project [Zahoree](https://infolink-exp.com/customer-experience-analytics/), when I started on the project it was a big data platform but with a a good amount of effort and work was able to change the direction of the project into a [customer experience](https://en.wikipedia.org/wiki/Customer_experience) optimization platform. Following this I won a position in [D-REAL](https://d-real.ie/) that will allow me to finance my PhD at [TU Dublin](https://www.tudublin.ie/).
