# Julia es técnica

![julia_dot_red_left](../../artefactos/imagenes/julia-dots_red_left.svg)

## Guia

```shell
>cd materiales_taller/julia_es_tecnica
>julia
```

### Crear un nuevo paquete

```julia-repl
julia>]
(@v1.7) pkg>generate SciPyLatam
```

```julia-repl
julia>;
shell>cd SciPyLatam
shell>ls -a
```

### Agregar tests

```julia-repl
julia>;
shell>mkdir test
shell>touch test/runtests.jl
```

```julia
using SciPyLatam
using Test

@testset "HOLA" begin
 @test f(1,2) == 5
end
```

### Importar desde otro projecto

```julia-repl
julia>]
pkg>add ../julia_es_tecnica/SciPyLatam
```

```julia-repl
julia>;
shell>git init
```

## Materiales adicionales

### **Videos**

- [Developing Julia Packages](https://www.youtube.com/watch?v=QVmU29rCjaA)
- [Package development in VSCode | Workshop](https://www.youtube.com/watch?v=F1R3ETaRQXY)
