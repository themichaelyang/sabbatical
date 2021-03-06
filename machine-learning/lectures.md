# Lecture Resources

## General

- Linear algebra: [MIT OCW Course — Excellent lecture notes!](https://ocw.mit.edu/courses/mathematics/18-06sc-linear-algebra-fall-2011/)
  - [Linear algebra review for Machine Learning (CMU)](http://www.cs.cmu.edu/~jingx/docs/linearalgebra.pdf)
- [Machine Learning (Coursera)](https://www.coursera.org/learn/machine-learning): can be useful to step back and see simpler explanations, practical considerations

## Lecture 2

- Gradient descent
  - [Do we need gradient descent to find the coefficients of a linear regression model? (Stack Exchange)](https://stats.stackexchange.com/questions/160179/do-we-need-gradient-descent-to-find-the-coefficients-of-a-linear-regression-mode/164164#164164)
  - Why simultaneous update? ["Why should we update simultaneously all the variables in gradient descent?" (Stack Exchange)](https://math.stackexchange.com/questions/2419301/why-should-we-update-simultaneously-all-the-variables-in-gradient-descent/2419310)
  - Mini-batch stochastic gradient descent: "*A compromise between computing the true gradient and the gradient at a single example is to compute the gradient against more than one training example (called a "mini-batch") at each step.*" [Wikipedia](https://en.wikipedia.org/wiki/Stochastic_gradient_descent)
  - Not mentioned: [Feature scaling (Coursera)](https://www.coursera.org/lecture/machine-learning/gradient-descent-in-practice-i-feature-scaling-xx3Da)
  - [Other optimization methods (Coursera)](https://www.coursera.org/learn/machine-learning/lecture/licwf/advanced-optimization)
- Linear regression
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
  - Ng brushes over this but seems pretty important. Some additional notes in the course website.
  - [Slides on convex optimization (Berkeley)](https://people.eecs.berkeley.edu/~jordan/courses/294-fall09/lectures/optimization/slides.pdf)
  - [Additional slides (NYU; not as clear)](https://cs.nyu.edu/~mohri/mls/ml_convex_optimization.pdf)
  - [Handout (CMU; have not fulled reviewed yet)](http://www.math.cmu.edu/~lohp/docs/math/mop2013/convexity-soln.pdf)

## Lecture 3

- Log Probability
  - Why log probability? [Explanation of log probability (Wikipedia)](https://en.wikipedia.org/wiki/Log_probability)
  - Review of log properties: [Derivations of log properties (Khan Academy)]( https://www.khanacademy.org/math/algebra2/exponential-and-logarithmic-functions/properties-of-logarithms/a/justifying-the-logarithm-properties)

## Lecture 4

- Newton's Method
  - ["Why is Newton's method not widely used in machine learning?" (Stack Exchange)](
https://stats.stackexchange.com/questions/253632/why-is-newtons-method-not-widely-used-in-machine-learning)
- Softmax regression
  - Derivation of gradient, relation to logistic regression: http://ufldl.stanford.edu/wiki/index.php/Softmax_Regression
http://ufldl.stanford.edu/tutorial/supervised/SoftmaxRegression/
- Generalized Linear Models (GLM)
  - More advanced treatment of GLM: [Generalized Linear Models (CMU)](http://www.stat.cmu.edu/~ryantibs/advmethods/notes/glm.pdf)
  - [Canonical link vs link function (Stack Exchange)](https://stats.stackexchange.com/questions/40876/what-is-the-difference-between-a-link-function-and-a-canonical-link-function)
  - We predict with the derived hypothesis model, $E[T(y);\eta]$. We assume that eta is linearly related: $\eta = \theta^Tx^{(i)}$. This assumption is known as the canonical link function (there are other ways to linearly relate the probability distribution).
  - This terminology comes from the exponential family's ["canonical form"](https://en.wikipedia.org/wiki/Exponential_family#Scalar_parameter).

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
- [The Spectrum Kernel: A String Kernel for Protein Classification](http://psb.stanford.edu/psb-online/proceedings/psb02/leslie.pdf)

## Lecture 9

- [Learning Theory slides (CMU)](https://www.cs.cmu.edu/~mgormley/courses/10601-s17/slides/lecture28-pac.pdf)
  - [Whiteboard content of slides](https://www.cs.cmu.edu/~mgormley/courses/10601-s17/slides/whiteboard28b.pdf)
  - Covers PAC learning (not covered by Ng)
- [PAC Learnable and Emperical Risk Minimization (Princeton)](http://www.cs.princeton.edu/~rlivni/cos511/lectures/lect2.pdf)
- For more in depth treatment:
  - [Machine Learning Theory (UCLA)](http://www.jennwv.com/courses/F11.html)

## Lecture 10

- Empirical risk minimization: 0-1 indicator loss function
  - SVM and logistic regression are convex approximations of ERM (so learning theory holds)
  - SVM: hinge loss
  - logistic regression: log loss
  - Some of the intuition relating the cost of SVM to logistic: [SVM Optimization Objectives (Coursera)]( https://www.coursera.org/lecture/machine-learning/optimization-objective-sHfVT)
- Not mentioned: Regularization (briefly discussed in lecture 11)
  - ISLR: Chapter 6, Linear Model Selection and Regularization

## Lecture 11

- [Prior probability (Wikipedia)](https://en.wikipedia.org/wiki/Prior_probability)
  - "In Bayesian statistical inference, a prior probability distribution, often simply called the prior, of an uncertain quantity is the probability distribution that would express one's beliefs about this quantity before some evidence is taken into account"
- [Posterior probability (Wikipedia)](https://en.wikipedia.org/wiki/Posterior_probability)
  - "In Bayesian statistics, the posterior probability of a random event or an uncertain proposition is the conditional probability that is assigned after the relevant evidence or background is taken into account."
- [Bayesian interpretation of Ridge and Lasso Regression (Princeton)](http://www.cs.princeton.edu/courses/archive/spr09/cos513/scribe/lecture10.pdf)
  - Interesting fact: [Uniform prior MAP degrades to MLE (Stack Exchange)](https://stats.stackexchange.com/questions/266415/if-we-have-a-uniform-prior-probability-distribution-across-all-ranges-of-thet)

## Tree Ensembles

- [Tree-based Methods Videos (Stanford)](https://lagunita.stanford.edu/courses/HumanitiesSciences/StatLearning/Winter2016/courseware/4cd5971758e84840b24d91c763df6ce8/bb3f21ec63554788b9a3023c22a98118/)
  - Pretty easy treatment of topic
  - Watch 5.4: Bootstrap before 8.4: Bagging
- Why Gini index and cross-entropy over classification error rate? Read Murphy: 16.2.2.2
  - In short: Gini and cross-entropy are more discriminant for tree purity (prioritize splits that contain fewer spread of classes), whereas 1-0 error fails to distinguish these cases
- [Errors and Residuals (Wikipedia)](https://en.wikipedia.org/wiki/Errors_and_residuals)
- Adaboost:

## Neural Networks
