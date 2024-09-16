# 定义域

```mathematica
A = ImplicitRegion[1 <= x^2 + y^2 <= 4, {x, y}];
B = ImplicitRegion[1 <= x^2 + y^2 + z^2 <= 4 && z >= 0, {x, y, z}];

```