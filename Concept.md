
# Autonomous

In a differential equation, autonomous means that the independent variable does not appear explicitly in the equation.

$$ \frac{dy}{dt} = f(y) $$

Here is an example contrasting autonomous and non-autonomous differential equations. In the following examples, the autonomous equation does not contain the independent variable t explicitly, whereas the non-autonomous equation does. However, this does not mean that y is not influenced by t in an autonomous equation. Even if y depends on t, that is, y = y(t), the equation can still be autonomous. It simply means that t does not appear explicitly in the differential equation itself.

- autonomous: $\frac{dy}{dt} = y^2 - 3y  \Leftrightarrow  \frac{dy(t)}{dt} = y(t)^2 - 3y(t)$
- non-autonomous:$\frac{dy}{dt} = 2t + y$

“Autonomous” comes from the Greek words auto (“self”) and nomos (“law”), meaning “self-governing.” In an autonomous differential equation, the evolution of the system is determined solely by its current state y, without explicit dependence on an external variable such as time t. This idea can be confusing at first, because y is still a function of t. However, the key point is that although y depends on t, the rate of change at any moment is determined only by the current state y, not by t itself. That is why the equation is called autonomous.

When a differential equation is autonomous, it is often easier to analyze the long-term behavior of the system. For example, in stability analysis, we can study what happens to the state as time goes to infinity. In equilibrium analysis, we can identify states at which the system stops changing by finding points where f(y)=0.

 # Complex number

I struggled to see the significance of complex numbers because they felt too 'imaginary' to be real. However, the same was once true for negative numbers. While 'two apples plus one' is intuitive, 'two apples plus negative one' seems impossible in the physical world; we can visualize zero apples, but not a negative amount. Yet, negative numbers became essential auxiliary tools to represent concepts like debt or opposite directions.

Similarly, complex numbers serve as an auxiliary system for real numbers. When mathematicians encountered the equation $x^2 = -1$, they realized that no real number could satisfy it, as squaring any real number results in a non-negative value. To resolve this logical gap, they devised the imaginary unit $i$, defined as the number whose square is $-1$.

Furthermore, they discovered that the imaginary unit represents a $90^{\circ}$ rotation. Since multiplying by $-1$ is equivalent to a $180^{\circ}$ rotation on the number line, the act of squaring $i$ to get $-1$ implies that multiplying by $i$ twice results in a $180^{\circ}$ turn. Therefore, a single multiplication by $i$ must correspond to a $90^{\circ}$ rotation, moving the number out of the 1D real line and into a 2D plane. Based on this concept, mathematicians devised the 'Complex Plane', where any number can be expressed in the rectangular form $a+bi$, which is equivalent to the coordinate $(a,b)$.

Likewise, just as a point $(x,y)$ in a rectangular coordinate system can be represented as $(r\cos\theta, r\sin\theta)$ using trigonometry, the complex number $(a,b)$ can also be expressed in terms of its distance $r$ from the origin and its rotation angle $\theta$. This results in the polar form: $r(\cos\theta + i\sin\theta)$. This shows that a complex number is not just a value, but a combination of magnitude and direction.

Mathematician Leonhard Euler favored the function $e^x$ because it is the only function that remains unchanged after differentiation. He wondered, 'What would happen if $x$ were replaced by the imaginary unit $ix$?'
He discovered a fascinating property: when $e^{ix}$ is differentiated twice, it becomes the negative of itself, as shown below.

- First derivative: $\frac{d}{dx}e^{ix} = i e^{ix}$ (A $90^{\circ}$ rotation)
- Second derivative: $\frac{d^2}{dx^2}e^{ix} = i^2 e^{ix} = -e^{ix}$ (A $180^{\circ}$ rotation, or the negative of itself)

This behavior perfectly mirrors the properties of $\sin(x)$ and $\cos(x)$, leading Euler to the realization that exponential growth and trigonometric rotation are deeply connected. Based on this insight, he utilized Taylor expansion to formally prove the identity: $e^{ix} = \cos(x) + i\sin(x)$ which is called **Euler's formula**.