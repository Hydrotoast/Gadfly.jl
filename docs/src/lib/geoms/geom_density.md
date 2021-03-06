```@meta
Author = "Daniel C. Jones"
```

# Geom.density

Draw a kernel density estimate from data. An alias for [Geom.line](@ref) with
[Stat.density](@ref).

## Aesthetics

  * `x`: Sample to draw density estimate from.

## Examples

```@setup 1
using RDatasets
using Gadfly
Gadfly.set_default_plot_size(14cm, 8cm)
```

```@example 1
plot(dataset("ggplot2", "diamonds"), x="Price", Geom.density)
```

```@example 1
plot(dataset("ggplot2", "diamonds"), x="Price", color="Cut", Geom.density)
```
