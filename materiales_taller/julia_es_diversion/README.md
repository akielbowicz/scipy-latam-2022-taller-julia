# Julia es diversión

![julia_dot_purple_right](../../artefactos/imagenes/julia-dots_purple_right.svg)

```shell
cd materiales_taller/julia_es_diversion
julia --project="."
```

```julia-repl
julia> using Pluto
julia> Pluto.run()
```

## Uso de PlutoUI

[PlutoUI](https://github.com/JuliaPluto/PlutoUI.jl)

```julia
using PlutoUI
```

```julia
@bind x Slider(1,2,10)
```

## Agregar paquetes locales

```julia
begin
 import Pkg
 Pkg.activate(".")
 Pkg.add(path="../julia_es_tecnica/SciPyLatam")
end
```
