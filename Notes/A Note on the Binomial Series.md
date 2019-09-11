# A Note on the Binomial Series

The [binomial series](https://www.encyclopediaofmath.org/index.php/Binomial_series)  

$$ \left( 1 + x \right)^n = \sum_{i=0}^n {n \choose i} 1^i x^{n-i} $$

can easily be proven to satisfy the following inequality under the assumption of $x \geq 0$:

$$ \sum_{i=0}^n {n \choose i} 1^i x^{n-i} \geq {n (n-1) \over 2} x^2 $$

which we have used in class during *Exercise 6, Problem 2 (iv)*.

### A Special Case

If we define a sequence $ x_n = \sqrt[n]{n} - 1$, then note that

$$ n = (1 + x_n)^n = \sum_{i=0}^n {n \choose i} 1^i x^{n-i} = 1 + x_n + {n (n-1) \over 2} x_n^2 + \ldots +x_n^n \qquad (*)$$

Then that the third term in the sequence is the lower bound we were trying to prove. Then, if we remove all additional terms, we obtain the required inequality.

For this, further note that $\forall n \in \mathbb{N}, n > 1$:

$$ \sqrt[n]{n} - 1 \leq 1 \iff \sqrt[n]{n} \leq 2 \iff n \leq 2^n $$

which is trivially true. Also:

$$ \sqrt[n]{n} - 1 > 0 \iff \sqrt[n]{n} > 1 \iff n > 1^n = 1 $$

which is also true given our assumption on $n$.

Thus the sum seen in $(*)$ is composed only of strictly positive terms. As such we have 

$$ 1 + x_n + {n (n-1) \over 2} x_n^2 + \ldots +x_n^n \geq {n (n-1) \over 2} x_n^2 $$

which yields the result. Indeed if we wanted we could tighten the "$\geq$" to a more strict "$>$" for $x_n > 0 \:\forall n$, too.	$\square$

#### Additional Sources

- https://www.encyclopediaofmath.org/index.php/Binomial_coefficients	"Binomial Coefficient"
- https://www.encyclopediaofmath.org/index.php/Binomial_series	"Binomial Series"
