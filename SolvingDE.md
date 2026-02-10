
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
