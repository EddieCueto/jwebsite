@def hascode = true

# Welcome to my blog

<!-- \tableofcontents  you can use \toc as well -->

This blog is where I intent to update my projects as well as my research. I am doing this right now due to COVID-19 and the fact that the epidemic started when I was about to start a PhD position in TU Dublin.
Currently I've been working in two "big" projects:
* `Setting up this blog` 
* `Implement compression methods for Deep Neural Networks Models (DNN)`.

Both of this projects are being developed with [Julia](https://julialang.org/), language which was introduced to my during my time at Instituto Politécnico Nacional - Center for Computing Research [IPN](https://www.cic.ipn.mx/index.php/es/). The Julia packages that I am either using or extending are [Flux.jl](https://fluxml.ai/) and [Franklin.jl](https://franklinjl.org/).

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

## Arriving to Dublin

OK it is been a while since I wrote on the blog, due to the (COVID-19) pandemic, the projects were maintained by me are on stand by and in 
need for an umdate now that Julia is on version 1.6.0 (it was 1.4.3 when they started) but I'm still working hard now into a more broader 
than just compressing a NN architecture. Now, models are so big their number of parameters is huge, just look at GPT-3; this has opened new
questions on the area specifically how "efficient" are the compression techniques when applied to those huge models.

Thanks to those theoretical advances now the previous problem of reducing the size of a model has become a multivariable optimization 
problem, where other hyperparameters influence the "efficiency" of how a model performs both during training, and inference. As an example,
we can mention the amount of FLOPS performed, the amount of energy consumed in Watts, clock time, etc. (all during training and inference).

This means that currently I am surveying SOTA models to compare if their gains on accuracy/precision are indeed valuable with respect the
previous, for example if the precision of a new model increments 0.0001 than former models but it consumes 100 times the amount of energy or
then that architecture is not efficient and should only be used on applications where that gain might be required. Also, I am exploring 
ideas from Topological Data Analysis to try and find smaller architectures that have as good performance and generalization as their more
parametrized counterparts.

Regarding my move to Dublin was a hassle...to arrive I had to take 3 flights one to Mexico City, then one to Dallas and finally to Dublin 
at least it wasn't as expensive due to COVID. I haven't been able to travel in Ireland, still on lockdown (08/04/2021) and might continue for
at least a month.

## A bit about myself

My interest in science started from a very early age I was in love with physics because a teacher in elementary school had a copy of the book `COSMOS` which he lend me and I was marveled by the words of [Carl Sagan](https://en.wikipedia.org/wiki/Carl_Sagan). A few years later I discovered chemistry and gave it a try but found it a bit expensive and hard so I kept trying to find "my calling", until as a teenager I got my first PC thanks to working in tending yards and some money that my parents were able to lend me.

It was an old HP machine that had installed Windows Me  ha,ha,ha one of the first things that I did was to open it to see how it was inside. After a few week, while browsing the web I read that there was something known as programming that allowed people to do stuff on computers, so a first attempt to learn to program was done in Basic and failed. In the following years due to some economical problems in my family I had to postpone my education for a few years, but was able to resume.

After my "sabbatical" I was able to finish a bachelor in mathematics which I loved, yes after some years I was able to find my calling and learned to program in C++ (which I don't use any more :P). But some of the biggest questions that I still have were not answered during my time in university. Mostly what is computation and why are there some problems harder to solve than others (some are even impossible to solve). So, as the very naive and curious person that I am, started a master in computer science and it was the best time of my life, living in one of the biggest cities of the world and working in one of the best research centers in Mexico [CIC-IPN](http://www.cic.ipn.mx/index.php/es/).

Finally in this last years I got a position as a lead data analyst on a machine learning project [Zahoree](https://infolink-exp.com/customer-experience-analytics/), when I started on the project it was a big data platform but with a a good amount of effort and work was able to change the direction of the project into a [customer experience](https://en.wikipedia.org/wiki/Customer_experience) optimization platform. Following this I won a position in [D-REAL](https://d-real.ie/) that will allow me to finance my PhD at [TU Dublin](https://www.tudublin.ie/).
