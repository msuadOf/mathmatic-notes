# 积分
see：[https://blog.csdn.net/BC_COM/article/details/105665193](https://blog.csdn.net/BC_COM/article/details/105665193)
## 三重积分

## 曲线积分
第一类曲线积分

第二类曲线积分

## 曲面积分
第一类曲面积分

第二类曲面积分
```mathematica
n = Grad[x^2 + y^2 + z^2, {x, y, z}];
f = {ArcTan[x/(y^2 + z^2)^(1/2)]/((y^2 + z^2)^(1/2)), 0, 
    0} . (n/Norm[n]);
A = ImplicitRegion[1 <= x^2 + y^2 + z^2 <= 4 && z >= 0, {x, y, z}];
Integrate[f, {x, y, z} \[Element] A]
```