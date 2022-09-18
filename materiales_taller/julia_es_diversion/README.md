# Julia es diversión

```shell
cd materiales_taller/julia_es_diversion
julia --project="."
```

```julia-repl
julia> using Pluto
julia> Pluto.run()
```

## Agregar paquetes locales

```julia
begin
 import Pkg
 Pkg.activate(".")
 Pkg.add(path="../julia_es_tecnica/SciPyLatam")
end
```
