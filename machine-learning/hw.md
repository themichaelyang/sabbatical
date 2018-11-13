# Homework Resources

## Problem Set 1

### Exercise 1
- Vectorizing / matrix form of some of the update rules are tough to derive on your own, especially the hessian
  - Includes design matrix in derivation: [Logistic regression - computing the Hessian (Youtube)]( https://www.youtube.com/watch?v=jUwjbiBUR-k&list=PLD0F06AA0D2E8FFBA&index=112)
  - [Hessian of logistic [objective] function (Stack Overflow)](https://stats.stackexchange.com/questions/68391/hessian-of-logistic-function)
- For question 3: plug in the probabilities and take the derivative with respect to each parameter and set to 0 (maximizing).
  - I think we can assume convexity
- For question 4:
  - Recall the multivariable chain rule: [Multivariable chain rule (Khan Academy)](https://www.khanacademy.org/math/multivariable-calculus/multivariable-derivatives/modal/a/multivariable-chain-rule-simple-version)
  - Review the linear algebra notes, especially the section on matrix calculus. The notation can get confusing, so make sure to read page 21. The official solution uses a more clear hessian notation, where: $H_f(y)$ is the Hessian of $f(\cdot)$ evaluated at point $y$.
  - Also, realize that the update rule of Newton's gives the formula to update on, but to actually do the update, you need to evaluate on the Hessian and matrix derivative.
  - The notation can get very confusing (parameters, values to evaluate on), so keep track of your symbols!
