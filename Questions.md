
# What does it mean to solve differential equation?

Normally, solving an equation means finding a solution that satisfies specific conditions. However, solving a differential equation is fundamentally different from solving an ordinary algebraic equation. In a differential equation, the equation specifies how the state(= (x,y)) of a system changes over time, rather than simply constraining its value. As a result, a solution is not just a single value, but an entire trajectory—a history of how the system evolves. Philosophically, solving an equation means predicting the future of a system by understanding the principle of causality.

In the context of the differential equation $y’ = f(x, y)$, solving a differential equation means finding a function $y(x)$ whose derivative matches $f(x, y)$

# What is the system?

A system is a set of variables that are connected to each other.

# Why do we need a initial value to solve differential equation?

Mathematically, solving a differential equation requires integration, which converts an equation for a derivative into an equation for the original function. Let us think in reverse. Suppose the original equation describing the history of $y$ is $y = x^2 + 3$. If we differentiate it, the constant disappears, giving $y’ = 2x$. Since integration is the inverse operation of differentiation, integrating $2x$ gives $x^2 + C$. However, the constant $C$ cannot be determined from the differential equation alone. To determine $C$, we need an initial condition (or initial state) for the differential equation. A problem given by a differential equation together with an initial value is called an Initial Value Problem (IVP).
