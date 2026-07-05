# Chapter 1. IDEAL FLUIDS

## $\S$ Equation of continuity

유체는 수많은 분자들로 이루어져있지만, 유체역학에서는 '물리적으로 작은' 유한한 요소에 집중한다. 
물리량들은 $\underline{u}(x,y,z,t) , p(x,y,z,t), \rho (x,y,z,t)$ 등으로 나타난다.

이제 제어공간 $V_0$ 를 고려해보자. 그 공간을 지나가는 유체의 질량은 $\int \rho dV$ 이다.
면적요소 $d\underline{f}$에서 단위시간당 이 공간을 지나는 유체의 질량은 $\rho \underline{u} \cdot d\underline{f}$ 이다. ($\frac{kg}{m^3} \frac{m}{s} m^2=\frac{kg}{s}$)
따라서  제어공간 $V_0$를 지나는 유체의 질량은

$$
\oint \rho \underline{u} \cdot d\underline{f} $$

제어공간  $V_0$의 단위시간당 감소하는 질량은 

$$
-\frac{\partial}{\partial t} \int \rho dV $$

앞서 언급한 내용과 같은 표현이므로, 

$$
-\frac{\partial}{\partial t} \int \rho dV=\oint \rho \underline{u} \cdot d\underline{f} $$

가우스의 발산정리 $^\dagger$에 의해 

$$
\oint \rho \underline{u} \cdot d\underline{f}=\int \nabla (\rho \underline{u})dV $$

$$
\int (\frac{\partial \rho}{\partial t}+\nabla (\rho \underline{u}))dV =0 \

\frac{\partial \rho}{\partial t}+\nabla (\rho \underline{u}) $$

이 식이 연속방정식(Equation of Continuity) 이다.

$\nabla (\rho \underline{u})=\rho \nabla underline{u}+\underline{u} \nabla \rho $ 로도 표현할수있으며

벡터 $\underline{j}=\rho \underline{u}$ 를 질량플럭스밀도 혹은 질량속도 (mass flux density)라고 표현한다.

---
$\dagger$ . 가우스의 발산정리

벡터 $\underline{r}(t)=x(t)\underline{i}+y(t)\underline{j}$ 에서 접선벡터는 $\frac{dx}{dt} \underline{i}+\frac{dy}{dt} \underline{j}$
법선벡터는 $\frac{dy}{dt} \underline{i}-\frac{dx}{dt} \underline{j}$

제어면적에서 어떤 벡터장 $\underline{F}=P d\underline{x}+Qd\underline{y}$ 이라고하면 제어면적의 법선벡터 $\underline{n}=d\underline{x}-d\underline{y}$ 이므로

내적하면 $\underline{F} \cdot \underline{n}=Pdx-Qdy$ . 
플럭스는
$\oint \underline{F} \cdot \underline{n} ds= \oint Pdx-Qdy $

그린의 정리에 의해 $\int \frac{\partial P}{\partial y}-(-\frac{\partial Q}{\partial x}) dA=\int \nabla \underline{F} dA$


