# Julia

```
using Pkg
Pkg.add("Conda")
using Conda

Conda.add("notebook")
ENV["JUPYTER"] = joinpath(Conda.BINDIR, "jupyter")
Pkg.build("IJulia")

using IJulia
notebook(detached=false)
```
