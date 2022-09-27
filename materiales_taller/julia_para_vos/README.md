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

En esta actividad pueden:

1. Definir una receta de plotting para graficar un tipo de dato propio con [RecipesBase.jl](https://github.com/JuliaPlots/RecipesBase.jl)

2. Explorar [UnicodePlots.jl](https://github.com/JuliaPlots/UnicodePlots.jl) para tener gráficos en la consola
o explorar [VegaLite.jl](https://github.com/queryverse/VegaLite.jl) para realizar plots interactivos.

3. Jugar haciendo imágenes con [Luxor.jl](https://github.com/JuliaGraphics/Luxor.jl) o animaciones con
[Javis.jl](https://github.com/JuliaAnimators/Javis.jl)

## Paquetes y librerías

En esta actividad pueden explorar la creación de un paquete usando un template con [PkgTemplates.jl](https://github.com/invenia/PkgTemplates.jl) que agrega las cosas necesarias de CI/CD, coverage, ...

## Interoperabilidad con Python

[PyCall.jl](https://github.com/JuliaPy/PyCall.jl)

## Programación Paralela y Distribuida

Esta actividad es para explorar las capacidades de Programación Paralela y distribuida
[Parallel Computing](https://docs.julialang.org/en/v1/manual/parallel-computing/)
usando [Distributed](https://docs.julialang.org/en/v1/stdlib/Distributed/) y [DistributedArrays.jl](https://github.com/JuliaParallel/DistributedArrays.jl)

Y si tienen GPU probar [CUDA.jl](https://github.com/JuliaGPU/CUDA.jl) y [GPUArrays.jl](https://github.com/JuliaGPU/GPUArrays.jl)

## Metaprogramación

Si se sienten aventureros y les interesa aprender a generar código que genera código pueden explorar
las capacidades de [Metaprogramación](https://docs.julialang.org/en/v1/manual/metaprogramming/) que tiene julia.
Adicionalmente están las librerías [MacroTools](https://github.com/FluxML/MacroTools.jl) con herramientas
predefinidas y [Cthulhu.jl](https://github.com/JuliaDebug/Cthulhu.jl) que ayuda a explorar el código generado
y facilita la búsqueda de errores.
