## linear-algebra.md

- [Linear algebra - Khan Academy](https://www.khanacademy.org/math/linear-algebra)

#### Vectors and spaces

###### [Vector dot product and vector length](https://www.khanacademy.org/math/linear-algebra/vectors-and-spaces/dot-cross-products/v/vector-dot-product-and-vector-length)

- Vector dot product calculated as `sum of products of respective components`
- Vector length: square root of sum of squares of individual components
- Vector length: also equals square root of the dot product of the vector with itself

###### [Dot and cross product comparison/intuition](https://www.khanacademy.org/math/linear-algebra/vectors-and-spaces/dot-cross-products/v/dot-and-cross-product-comparison-intuition)

- Dot product: product of a vector and the component of other on it
- Dot product is 0 if the vectors are perpendicular, product of magnitudes if the vectors are colinear
- Cross product: product of a vector and the perpendicular component of the other
- Cross product is the product of magnitudes if the vectors are perpendicular, 0 if the vectors are colinear


## [Essence of linear algebra - 3Blue1Brown](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)

###### Linear Algebra

- language to describe space and the manipulation of space



##### 1. Vectors, what even are they?

###### Vectors

- geometrically, can be thought of as an arrow in a coordinate system where the head sits at the point indicated by the vector & the tail sits at the origin 

###### Vector Addition

- can be thought of as combining movements (in space) 
- numerically, it is determined by adding the respective components 

###### Scalar Multiplication

- can be thought of a 'scaling' (stretching or squishing) operation
- numerically, it is determined by multiplying every component with the scalar

##### 2. Linear combinations, span, and basis vectors

###### Basis Vectors

- if each coordinate/component is a vector can be thought of as a scalar multiplied by unit vectort (in that direction), then the vector itself can be thought of as their sum
- these unit vectors are called 'basis vectors' 
- represented as i-hat & j-hat

###### Linear Combination

- operation of scaling vectors and adding them

###### Span

- set of all linear combinations

###### Linearly Dependent

- one of the vectors doesn't add any new dimention to the span, or
- one of the evctors can be expressed as a linear combination of the others

###### Basis of a vector space

- technically defined as a set of linearly independent vectors that span that vector space 

##### 3. Linear transformations and matrices

###### Linear transformation

- can be thought of as a function being applied to a vector to obtain a new vector
- with the condition that, all lines are parallel & equally spaced
- in 2 dimensions, the result of a transformation can be determined by two coordinates: coordinates where i-hat & j-hat land
- a 'transformation' is therefore a packaging of final positions of i-hat & j-hat in a 2x2 matrix where the columns describe the position of i & j 
- matrices therefore can be thought of as 'transformations' being packaged such that the columns tells us where the corresponding basis vector lands after the transformation
- matrix multiplication can be thought of as applying a transformation to a vector
- numerically, it is simply adding the scaled versions of basis vectors


#### 4. [Matrix multiplication as composition](https://youtu.be/XkY2DOUCWMU)

- multiplying two matrices is geometrically the same as applying one transformation and then the other
- the order of multiplication is right to left (transformation represented by the right matrix is applied first)

###### Calculating the product of two matrices

- where does i-hat land after the first transformation? `1st col of 2nd matrix`
- where does i-hat land after the second transformation? `(2nd matrix) * (1st col of 2nd matrix)`
- this is the same as the first column of the result!
- similarly obtain the second column of result

## [Linear Algebra - MIT OCW](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/)

- [MIT 18.06 Linear Algebra, Spring 2005 - YouTube](https://www.youtube.com/playlist?list=PLE7DDD91010BC51F8)

#### [1. The geometry of linear equations](https://youtu.be/ZK3O402wf1c)

- `Ax = b` Ax is a combination of columns of A, or
- `Ax = b` the columns of A scaled by x produces b

