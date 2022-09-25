# Julia es practicidad

![julia-dots-green-top](../../artefactos/imagenes/julia-dots_green_top.svg)

En esta primera actividad vamos a ver un poco la sintaxis de `julia`
y como se asemeja y difiere de la de `python`.

## Trabajando en `Jupyter`

Para aprender sobre `julia` en un territorio conocido vamos a trabajar desde cuadernos de
`jupyter`.

Primero vamos a iniciar una `REPL` o consola de `julia` en la carpeta de esta actividad.

```shell
> cd materiales_taller/julia_es_practicidad
> julia --project="."
```

Si todo esta instalado bien, una vez que inicialicemos `julia` deberiamos ver el mensaje introductorio:

```shell
               _
   _       _ _(_)_     |  Documentation: https://docs.julialang.org
  (_)     | (_) (_)    |
   _ _   _| |_  __ _   |  Type "?" for help, "]?" for Pkg help.
  | | | | | | |/ _` |  |
  | | |_| | | | (_| |  |  Version 1.7.3 (2022-05-06)
 _/ |\__'_|_|_|\__'_|  |  Official https://julialang.org/ release
|__/                   |

julia> 
```

Para poder trabajar desde `jupyter` necesitamos instalar [IJulia](https://github.com/JuliaLang/IJulia.jl), que en el caso de ya tener instalado `jupyter` va a crear un **kernel** para `julia` y en caso de no tenerlo nos va a preguntar si queremos instalarlo usando `conda`.

```julia-repl
julia> using IJulia
```

Una vez que la instalación termine, para abrir `jupyter lab` ejecutamos

```julia-repl
julia> jupyterlab(dir=".")
```

O en caso de los `notebooks` tradicionales, podemos ejecutar

```julia-repl
julia> notebook(dir=".")
```

Ya en `jupyter`, abran el cuaderno `julia_es_practicidad.ipynb`

## Uso de Librerias

- [Plots](https://docs.juliaplots.org/latest/)
- [StatsPlots](https://docs.juliaplots.org/latest/generated/statsplots/#StatsPlots)
- [DataFrames](https://dataframes.juliadata.org/stable/man/getting_started/)
- [CSV](https://csv.juliadata.org/stable/)

```julia-repl
import Pkg
pkg"add Plots, DataFrames"
```

### Uso de [PlotlyJS.jl](https://juliaplots.org/PlotlyJS.jl/stable/) para gráficos interactivos

```julia-repl
pkg"add PlotlyJS"
```

En algunos casos hay que agregar extensiones adicionales para que `Plotly`
funcione correctamente en `Jupyter`

```julia-repl
using Conda
Conda.pip_interop(true)
Conda.pip("install", "webio_jupyter_extension")
```

Y en `jupyter lab` también puede que sea necesario ejecutar lo siguiente

```shell
> conda activate "PATH de conda"
> jupyter labextension install jupyterlab-plotly
```

## Materiales adicionales

- Lista de diferencias especificas con otros lenguajes como Python, Matlab, R ... [Noteworthy differences](https://docs.julialang.org/en/v2/manual/noteworthy-differences/)
