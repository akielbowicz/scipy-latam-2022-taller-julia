# Actividades para practicar

![julia-dots](../../artefactos/imagenes/julia-dots.svg)

Ahora que ya saben lo básico de como trabajar en `julia` pueden explorar
las siguentes propuestas de actividades.

[JuliaHub](https://juliahub.com/ui/Packages)

## Performance

Una de las características más valoradas de `julia` es la performance, y algo
muy importante es la infraestructura para poder evaluarla.

En esta actividad podés:

1. Realizar un benchmark de alguna de las funciones implementadas y responder las siguentes
preguntas

2. Reimplementar una función que use un ciclo `for` usando *broadcasting* o viceversa y
compararlas con un benchmark.

3. Estudiar cual es el *hot path* de la función en cada caso y evaluar en que se puede optimizar.
Es una cuestion de poder de procesamiento (CPU), o algo de memoria?

Las librerías que te pueden llegar a ser útiles.
[BenchmarkTools.jl](https://github.com/JuliaCI/BenchmarkTools.jl)
[Profile](https://docs.julialang.org/en/v1/stdlib/Profile/)
[FlameGraphs.jl](https://github.com/timholy/FlameGraphs.jl)
[ProfileView](https://github.com/timholy/ProfileView.jl)

## Ecuaciones Diferenciales

El ecosistema de resolución de Ecuaciones Diferenciales de `julia` es uno de los
m'as completos y poderosos que existen.

En esta actividad podes:

1. Plantear una ecuaci[on diferencial de primer orden y una sola variable de la cual conozcas la solucion
anal[itica y resolverla de manera num[erica y compararlas en un gr[afico.

2. Estudiar los distintos métodos (Euler, Runge-Kutta, ...) que están disponibles en
las libreria.

3. Extender a un sistema de ecuaciones diferenciales lineales de 3 o más componentes y graficar la
solucion

4. Probar con un sistema de 100 dimensiones

[DifferentialEquations.jl](https://github.com/SciML/DifferentialEquations.jl)
[ModelingToolkit.jl](https://github.com/SciML/ModelingToolkit.jl)
[DiffEqFlux.jl](https://github.com/SciML/DiffEqFlux.jl)

## Aprendizaje Automático

[Flux.jl](https://github.com/FluxML/Flux.jl)
[MLJ.jl](https://github.com/alan-turing-institute/MLJ.jl)

## Gráficos y visualizaciones

[RecipesBase.jl](https://github.com/JuliaPlots/RecipesBase.jl)

[UnicodePlots.jl](https://github.com/JuliaPlots/UnicodePlots.jl)
[VegaLite.jl](https://github.com/queryverse/VegaLite.jl)

[Luxor.jl](https://github.com/JuliaGraphics/Luxor.jl)
[Javis.jl](https://github.com/JuliaAnimators/Javis.jl)

## Paquetes y librerías

[PkgTemplates.jl](https://github.com/invenia/PkgTemplates.jl)

## Programación Paralela y Distribuida

[Parallel Computing](https://docs.julialang.org/en/v1/manual/parallel-computing/)

[CUDA.jl](https://github.com/JuliaGPU/CUDA.jl)
[GPUArrays.jl](https://github.com/JuliaGPU/GPUArrays.jl)

[Distributed](https://docs.julialang.org/en/v1/stdlib/Distributed/)
[DistributedArrays.jl](https://github.com/JuliaParallel/DistributedArrays.jl)

## Metaprogramación

[Metaprogramación](https://docs.julialang.org/en/v1/manual/metaprogramming/)
[MacroTools](https://github.com/FluxML/MacroTools.jl)
[Cthulhu.jl](https://github.com/JuliaDebug/Cthulhu.jl)

## Interoperabilidad con Python

[PyCall.jl](https://github.com/JuliaPy/PyCall.jl)
