
# How to solve differential equation?

## Separation of Variables

The difficulty of solving a differential equation comes from the fact that x and y are entangled. In fact, the goal of solving an ordinary differential equation is often to rewrite it in a form with separated variables. 

This raises the question: "Why do entangled variables make problems difficult to solve?". Consider the following expression. Suppose that y depends on x, but the functional relationship between them is unknown. If we attempt to compute.

$ \int{xy}dx$

The expression x y is difficult to integrate because the dependence of y on x is unknown. Therefore, we use the method of separation of variables to solve the differential equation.

## Substitution

The substitution method is a technique to achieve a goal for separation of variables. Consider the following equation

$$ \frac{dy}{dx} = (x + y)^2 $$

This equation is difficult to solve directly because the variables x and y are entangled in the term (x+y), which prevents direct separation of variables.

We can simplify the problem using the substitution method. Let u = x + y and substitute it into the equation. The right-hand side can then be written easily as u^2. However, we must also rewrite the left-hand side in terms of u. To do this, we find the relationship between $\frac{du}{dx}$ and $\frac{dy}{dx}$ by differentiating both sides of the substitution:

1. $u = x + y$
2. $\frac{du}{dx} = \frac{dx}{dx} + \frac{dy}{dx}$
3. $\frac{dy}{dx} = \frac{du}{dx} - 1 $

Now, we have all the ingredients to apply the substitution method. 

1. Substitution: $ \frac{du}{dx} - 1 = (u^2) $ -> $ \frac{du}{dx} - 1 = (u^2) $
2. Separation of variables: $\frac{1}{u^2 + 1}{du} = dx $

## How to solve ODE after finding integrating factor?

After finding an integrating factor, we multiply it on both sides of the equation. This transforms the equation into a form that can be written as a derivative. Then, we integrate the equation to find the solution.

Here is the procedure for the procedure for solving a first-order linear ODE

1. Convert the ODE into the standard linear form.
    - $y' + p(x)y = q(x)$
2. Find the integrating factor.
    - $u = e^{\int{p(x)}dx}$
3. Multiply both sides of the equation by the integrating factor.
    - $uy' + up(x)y = u(x)q(x)$
4. Rewrite the left-hand side as a derivative
    - $(uy)' = q(x)u$
5. Integrate both sides.
    - $\int{(uy)'} = uy + C = \int{q(x)u}dx + C$
6. Find the solution.
    - $y = \frac{\int{qu}dx}{u}$

Let's solve this equation by the above procedure: $ xy' - y = x^3 $.

- First, we need to convert the equation into the standard linear form: $y' -\frac{1}{x}y = x^2$
- Second, let's find the integrating factor: $u = e^{-(\int{\frac{1}{x}}dx)} = (e^{ln(x)})^{-1} = \frac{1}{x}$.
- Third, multiply both sides of equation by the integrating factor: $\frac{1}{x}y' - \frac{1}{x^2}y = x$
- Fourth, rewrite the left side as as derivatve: $(\frac{1}{x}y)' = x$
- Fifth, integrate both sides: $\frac{1}{x}y = \frac{1}{2}x^2 + C$
- Sixth, find the solution: $y = \frac{1}{2}x^3 + Cx$
