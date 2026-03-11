
# Autonomous

In a differential equation, autonomous means that the independent variable does not appear explicitly in the equation.

$$ \frac{dy}{dt} = f(y) $$

Here is an example contrasting autonomous and non-autonomous differential equations. In the following examples, the autonomous equation does not contain the independent variable t explicitly, whereas the non-autonomous equation does. However, this does not mean that y is not influenced by t in an autonomous equation. Even if y depends on t, that is, y = y(t), the equation can still be autonomous. It simply means that t does not appear explicitly in the differential equation itself.

- autonomous: $\frac{dy}{dt} = y^2 - 3y  \Leftrightarrow  \frac{dy(t)}{dt} = y(t)^2 - 3y(t)$
- non-autonomous:$\frac{dy}{dt} = 2t + y$

“Autonomous” comes from the Greek words auto (“self”) and nomos (“law”), meaning “self-governing.” In an autonomous differential equation, the evolution of the system is determined solely by its current state y, without explicit dependence on an external variable such as time t. This idea can be confusing at first, because y is still a function of t. However, the key point is that although y depends on t, the rate of change at any moment is determined only by the current state y, not by t itself. That is why the equation is called autonomous.

When a differential equation is autonomous, it is often easier to analyze the long-term behavior of the system. For example, in stability analysis, we can study what happens to the state as time goes to infinity. In equilibrium analysis, we can identify states at which the system stops changing by finding points where f(y)=0.

 