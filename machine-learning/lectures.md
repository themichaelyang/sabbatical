# Lecture Resources

## General

- Linear algebra: [MIT OCW Course — Excellent lecture notes!](https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/)
  - [Linear algebra review for Machine Learning (CMU)](http://www.cs.cmu.edu/~jingx/docs/linearalgebra.pdf)
- [Machine Learning (Coursera)](https://www.coursera.org/learn/machine-learning): can be useful to step back and see simpler explanations, practical considerations

## Lecture 2

### Gradient descent
- Why simultaneous update? ["Why should we update simultaneously all the variables in gradient descent?" (Stack Exchange)](https://math.stackexchange.com/questions/2419301/why-should-we-update-simultaneously-all-the-variables-in-gradient-descent/2419310)
- Mini-batch stochastic gradient descent: "*A compromise between computing the true gradient and the gradient at a single example is to compute the gradient against more than one training example (called a "mini-batch") at each step.*" [Wikipedia](https://en.wikipedia.org/wiki/Stochastic_gradient_descent)

### Linear regression

- Linear regression to fit nonlinear functions: ["Can a linear regression be quadratic?" (Stack Exchange)](https://math.stackexchange.com/questions/2022783/can-a-linear-regression-be-quadratic)
- Least squares review from linear algebra:
  - [Lecture notes (MIT OCW)](https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/least-squares-determinants-and-eigenvalues/projection-matrices-and-least-squares/MIT18_06SCF11_Ses2.3sum.pdf)
  - [Videos and materials (MIT OCW)]( https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/least-squares-determinants-and-eigenvalues/projection-matrices-and-least-squares/)
- See also: ESL2, Section 3.2 (pg 45)
  - [Why is y−ŷ perpendicular to the subspace spanned by x in linear regression? (Stack Exchange)]( https://stats.stackexchange.com/questions/241025/why-is-mathbfy-mathbf-haty-perpendicular-to-the-subspace-spanned-by)
  - [Why is $X^TX$ invertable? (Reddit)]( https://www.reddit.com/r/MachineLearning/comments/3ilhnv/why_is_xt_x_invertible/)
  - [Proof that any positive definite is invertible (Stack Exchange)](https://math.stackexchange.com/questions/1059566/explain-proof-that-any-positive-definite-matrix-is-invertible)
- [Why use gradient descent for linear regression, when a closed-form math solution is available? (Stack Exchange)](https://stats.stackexchange.com/questions/278755/why-use-gradient-descent-for-linear-regression-when-a-closed-form-math-solution)

- Convex optimization (proof of convergence of linear regression):
  - Ng brushes over this but seems pretty important. Looking at syllabus, might be covered later?
  - [Slides on convex optimization (Berkeley)](https://people.eecs.berkeley.edu/~jordan/courses/294-fall09/lectures/optimization/slides.pdf)
  - [Additional slides (NYU; not as clear)](https://cs.nyu.edu/~mohri/mls/ml_convex_optimization.pdf)
  - [Handout (CMU; have not fulled reviewed yet)](http://www.math.cmu.edu/~lohp/docs/math/mop2013/convexity-soln.pdf)

## Lecture 3

### Log Probability
- Why log probability? [Explanation of log probability (Wikipedia)](https://en.wikipedia.org/wiki/Log_probability)
- Review of log properties: [Derivations of log properties (Khan Academy)]( https://www.khanacademy.org/math/algebra2/exponential-and-logarithmic-functions/properties-of-logarithms/a/justifying-the-logarithm-properties)

## Lecture 4

### Newton's Method
- ["Why is Newton's method not widely used in machine learning?" (Stack Exchange)](
https://stats.stackexchange.com/questions/253632/why-is-newtons-method-not-widely-used-in-machine-learning)

### Softmax regression
- Derivation of gradient, relation to logistic regression: http://ufldl.stanford.edu/wiki/index.php/Softmax_Regression
http://ufldl.stanford.edu/tutorial/supervised/SoftmaxRegression/

## Lecture 5

- https://ai.stackexchange.com/questions/2106/how-can-one-intuitively-understand-generative-v-s-discriminative-models-specifi
- Covariance: *"If the greater values of one variable mainly correspond with the greater values of the other variable, and the same holds for the lesser values, (i.e., the variables tend to show similar behavior), the covariance is positive. In the opposite case, when the greater values of one variable mainly correspond to the lesser values of the other, (i.e., the variables tend to show opposite behavior), the covariance is negative. The sign of the covariance therefore shows the tendency in the linear relationship between the variables. The magnitude of the covariance is not easy to interpret because it is not normalized and hence depends on the magnitudes of the variables. The normalized version of the covariance, the correlation coefficient, however, shows by its magnitude the strength of the linear relation."*  [Wikipedia](https://en.wikipedia.org/wiki/Covariance)
- [Linear methods for classification (UMD)](http://users.umiacs.umd.edu/~hcorrada/PracticalML/pdf/lectures/classification.pdf)
  - Useful notes on Linear (Gaussian) Discriminant Analysis

## Lecture 6

- [Multinomial distribution  (Wikipedia)](https://en.wikipedia.org/wiki/Multinomial_distribution)
- [Decision boundary of logistic regression (Coursera)](https://www.coursera.org/lecture/machine-learning/decision-boundary-WuL1H)
  - Useful for intuition of linear boundary of logistic regression
- Why is the weight vector is orthogonal to the separating hyperplane $(w^t * x + b = 0)$?
  - [Normals to Planes and Lines (UW)]( http://sites.math.washington.edu/~king/coursedir/m445w04/notes/vector/normals-planes.html)
  - [Review: Normal vector from plane equation (Khan Academy)](https://www.khanacademy.org/math/linear-algebra/vectors-and-spaces/dot-cross-products/v/normal-vector-from-plane-equation)

# Lecture 7

- [SVM Notes (NYU) ](https://davidrosenberg.github.io/mlcourse/Labs/3-SVM-Notes_sol.pdf)
  - "Hard Margin SVM" Section gives a simpler derivation and better intuition of why we have to impose constraint on max geometric margin problem (since $w$ and $b$ can be scaled even dividing by magnitude)
  - Why does Ng use the functional margin over the geometric margin when formulating the optimization problem? Is this because the final result optimizes this property? I'm assuming this has to do with the functional margin being a convex problem.
  - Additionally, why do we care about constraining $w$ and $b$ if we will get the hyperplane regardless? Or will not constraining not give us a convex problem?
- [SVM Slides (NYU / MIT)](http://people.csail.mit.edu/dsontag/courses/ml13/slides/lecture3.pdf)
  - Notice how boundary doesn't change regardless of scaling factor!
- [SVM Slides (CMU)](https://www.cs.cmu.edu/~tom/10701_sp11/slides/Kernels_SVM2_04_12_2011-ann.pdf)
- [Why do we choose to minimize ${1\over{2}}||w||^2$ instead of maximizing $1\over{||w||}$? (Stack Exchange) ](https://math.stackexchange.com/questions/1815810/why-do-we-minimize-the-squared-norm-instead-of-the-norm-in-this-optimization-pro)
- [How is maximizing $1\over{||w||}$ equivalent to minimizing ${1\over{2}}||w||^2$? (Stack Exchange) ](https://math.stackexchange.com/questions/773847/why-is-max-frac2w-min-frac12w2)
- [Positive Definite Matrices](https://www.math.utah.edu/~zwick/Classes/Fall2012_2270/Lectures/Lecture33_with_Examples.pdf)
- [Matrix Cookbook](https://www.math.uwaterloo.ca/~hwolkowi/matrixcookbook.pdf)
- [Deriving the optimal value for the intercept term in SVM (Stack Exchange)](https://stats.stackexchange.com/questions/91269/deriving-the-optimal-value-for-the-intercept-term-in-svm)

## Lecture 8

- Why does polynomial kernel ($K(x,z) = (x^Tz + c)^d$) map to a ${n+d \choose d}$ space?
  - I believe we can think of this as choosing $d$ number of $x$ terms from the set of $x_1, x_2... x_n$, repeated $d$ times, since $(x_1)^d$ is possible. We use combination because we want the unique terms to find the feature space; the length of the vector given by $\phi(x)$ includes duplicate terms (e.g. $x_1x_2$ and $x_2x_1$ in the basic kernel).
  - Less intuitive answer: [Polynomial kernel feature space (Stack Exchange)](https://stats.stackexchange.com/questions/285292/polynomial-kernel-feature-space)
- [Hinge loss (Wikipedia)](https://en.wikipedia.org/wiki/Hinge_loss)
  - Ng doesn't talk about this and only briefly mentioned in supplemental notes, also generally skips over cost functions
  - [Constrained versus unconstrained formulation of SVM optimization (Stack Exchange)]( https://stats.stackexchange.com/questions/6637/constrained-versus-unconstrained-formulation-of-svm-optimisation)
  - [SVM Slides (Oxford, pg 29 for hinge loss)](http://www.robots.ox.ac.uk/~az/lectures/ml/lect2.pdf)
  - [SVM Intuitive Explanation (Coursera)](https://www.coursera.org/lecture/machine-learning/optimization-objective-sHfVT)
