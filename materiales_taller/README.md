# Pre requisitos

- **Instalar Julia**

La manera recomendada es usando [juliaup](https://github.com/julialang/juliaup#juliaup---julia-version-manager)

En Windows (necesitan [winget](https://learn.microsoft.com/en-us/windows/package-manager/winget/#install-winget))

```powershell
> winget install julia --source msstore
```

En Linux/MacOS

```fish
> curl -fsSL https://install.julialang.org | sh
```

- **Editor de código**

Preferente, [Visual Studio Code](https://code.visualstudio.com/)

```powershell
> winget install --id Microsoft.VisualStudioCode --source winget
```

O usando [Scoop](https://scoop.sh/)

```powershell
> scoop bucket add extras
> scoop install vscode
```

Para Vim existe el paquete de [julia-vim](https://github.com/JuliaEditorSupport/julia-vim/blob/master/INSTALL.md)
