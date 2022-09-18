# Julia es practicidad

![julia-dots-green-top](../../artefactos/imagenes/julia-dots_green_top.svg)

## Guia

```shell
> julia --project="."
```

```julia-repl
julia> using IJulia
julia> jupyterlab(dir=".")
```

## Uso de Librerias

- Plots
- DataFrames

```julia-repl
import Pkg
pkg"add Plots, DataFrames"
```

```julia-repl
using Conda
Conda.pip_interop(true)
Conda.pip("install", "webio_jupyter_extension")
```

Alternativamente

```shell
> conda activate "PATH de conda"
> jupyter labextension install jupyterlab-plotly
```

```julia-repl
julia> notebook(dir=".")
```


## Materiales adicionales

- Lista de diferencias especificas con otros lenguajes como Python, Matlab, R ... [Noteworthy differences](https://docs.julialang.org/en/v2/manual/noteworthy-differences/)