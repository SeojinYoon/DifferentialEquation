
# What is ODE?

The differential equation(DE) describes the direction and rate of change of a system given its current state. An ordinary differential equation(ODE) does this with respect to a single independent variable.

## What is the difference between DE and Equation?

An equation defines a constraint (relation) between variables. In contrast, a differential equation (DE) describes a rule governing how a dependent variable changes with respect to an independent variable.

Solving an equation means finding all possible states (points) that satisfy the given constraint. In contrast, solving a DE means finding a function (or a family of functions) whose derivative satisfies the given rule.

Consider the equation x^2 + y^2 = 4. Its solution $\{(x,y)\in\mathbb{R}^2 \mid x^2 + y^2 = 4\}$ is the set of all states (x,y) satisfying the equation.Now consider the differential equation y' + 2x = 4. Its solution is $y(x) = 4x - x^2 + C$ ,which represents a family of functions describing the possible state trajectories of y as a function of x.

If the independent variable is time, the solution of a DE can be interpreted as the time evolution (trajectory) of a system given an initial condition. Philosophically, solving a differential equation corresponds to predicting the future behavior of a system based on its governing dynamics and the principle of causality.

# Are the symbols y and f the same in y' = f(x,y)?

No, The symbols y and f are different. The symbol f represents a rule that combines x and y to determine how the system changes.

For example, consider the equation. $ y' = f(x, y) $. If we int erpret the y' as the gradual change of position with respect to time, the y represents position and x represents time. The function f describes how the current state (x,y) determines this rate of change.

Thus, f is the mechanism of a two-variable state system, and y' is the output of that system, representing how the position changes at a given time and location.

# What is the system?

A system is a set of variables that are connected to each other.

# Why do we need a initial value to solve differential equation?

Mathematically, solving a differential equation requires integration, which converts an equation for a derivative into an equation for the original function. Let us think in reverse. Suppose the original equation describing the history of $y$ is $y = x^2 + 3$. If we differentiate it, the constant disappears, giving $y’ = 2x$. Since integration is the inverse operation of differentiation, integrating $2x$ gives $x^2 + C$. However, the constant $C$ cannot be determined from the differential equation alone. To determine $C$, we need an initial condition (or initial state) for the differential equation. A problem given by a differential equation together with an initial value is called an Initial Value Problem (IVP).

Let's consider this equation. $ a(x)y' + b(x)y = c(x) $

# What is standard linear form?

The standard linear form is a clear and standardized way to represent a first-order linear differential equation so that it can be solved systematically. This form provides a systematic view by separating the system the system dynamics $p(x)$ from the external input $Q(x)$. The term $p(x)y$ represents the rate of change depending on current state, whereas $q(x)$ represents an external input that is independent of the current state.

It has the form $ \frac{dy}{dx} + p(x)y = q(x) $ 

This form satisfies the following conditions.
1. The coefficient of $\frac{dy}{dx}$ is 1.
2. The term involving y appears on the left-hand side.
3. The term depending only on x appears on the right-hand side.

## Why do we convert the DE into a standard linear form?

In the stardard linear form, we can solve the equation mechanically using a method called intergral factor. Here is the integrating factor $ μ(x) = e^{\int{p(x)}dx} $. 

### Where the integrating factor come frome?

The integrating factor is a function introduced to transform a first-order linear differential equation into the derivative of a product (via the product rule).

Let me explain this in detail. Consider the standard linear form: $y' + p(x)y = q(x)$, we multiply both sides by a function $u(x)$, obtaining $uy' + p(x)uy = q(x)u$. Using the product rule, $(uy)' = uy' + u'y = q(x)u$. To rewrite the left-hand side as $q(x)u$, we require $ u' = p(x)u $. This differential equation can be solved by separation of variables: $\frac{1}{u}du = p(x)dx $. Integrating both side gives $ln(u) = \int{p(x)}dx$ and therefore, $u = e^{\int{p(x)}dx}$.

# What is the difference between homogenous and inhomogenous?

A differential equation is **homogeneous** if all terms involve the dependent variable and its derivatives only (no standalone independent variable), so the equation can be written with zero on the right-hand side. In contrast, a differential equation is **inhomogenous** if it contains a term that is independent of the dependent variable, so it can be written with non-zero from on the right-hand side. Here is the example of homogenous and inhomogenous equation.

Examples:
- homogenous: $y'' + 3y' + 2y = 0$ 
- inhomogenous $y'' + 3y' + 2y = 3$

One might raise the question that, in the homogeneous example, the term 0 does not involve the dependent variable and therefore the equation should not be considered homogeneous. However, the zero term can be written as $0 \cdot y$, which involves the dependent variable. Thus, the equation is indeed homogeneous.

# Various kinds of solutions of DE

There are many kinds of solutions when solving differential equation. In this section, I will explain two kinds of solutions: The general solution and the particular solution. The general solution represents a framework of solutions that includes all possible solutions of DE. To solve a differential equation, we perform integration, which introduces an unknown integration constant. Because the value of this constant is not specified, the solution can take different forms. A solution that retains this arbitrary constant is called the **general solution**, whereas a solution in which the constant is specified using additional conditions is called a **particular solution**.

## The number of integral constants

For a first-order linear homogeneous differential equation, the general solution has the form
$y(x) = C_{1} y_{1}(x).$

In contrast, for a second-order linear homogeneous differential equation, the general solution is given by
$y(x) = C_{1} y_{1}(x) + C_{2} y_{2}(x).$

Comparing these two forms, one may ask why the number of integration constants increases with the order of the differential equation. The reason is that solving a first-order differential equation requires one integration, whereas solving a second-order differential equation requires two integrations. Each integration introduces one integration constant, leading to an additional constant in the general solution.


