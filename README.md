# How-to-Talk-Linear-Algebra-Review-2

December 25, 2020

I appreciate comments. Shoot me an email at noel_s_cruz@yahoo.com!

Hire me! 😊

- We now continue our review of linear algebra.
Last time, we looked at the dot product between two vectors.
What we'll do today is to build upon this
to get products between vectors and matrices
and matrices and matrices.
This is crucial to modeling linear functions,
which are among the most common functions
that we'll be using in this class.
So what are linear functions?
And while we're at it, what are quadratic functions?
Well, in one dimension, a linear function of one variable X
is something like three X plus two.
And a quadratic function is similar,
except that it's also allowed to have a squared term.
So it can be something like
four X squared minus two X plus six.
But what about in higher dimension?
Let's say we're in three dimensions, for instance.
In this case, a linear function is a sum
of a bunch of terms,
and each term is either a constant, like four,
or it's just a multiple of one of the variables.
So we end up with something like
three X one minus two X two plus X three plus four.
A quadratic function is also just a sum of terms,
and each term is either a constant, or a linear term,
or it could be the square of one of the variables
like X one squared or six X two squared.
Or it could use the pairwise product
of two of the variables, like this term over here,
minus two X one X three, okay?
So this is what linear and quadratic functions are
for higher dimensional data.
Now, we'll be making very heavy use of linear functions.
For instance, a lot of the methods we study
support vector machines, logistic regressions, and so on
are based on linear decision boundaries, okay?
What exactly are these?
Well, suppose we have data in two dimensional space,
then a linear decision boundary's just a line,
something like the line showed over here.
And what we would do with this decision boundary
is one side of the boundary would be classified as plus
and the other side would be classified as minus.
Now, what is the equation of a linear boundary like this?
Well, this is in two D so it's just a line
and this particular line has the following equation.
Four X one plus three X two equals 12.
Let's check this, okay?
So this is the X one direction here,
this is the X two direction.
Let's check this particular point.
So this is the point three zero.
Does it lie on this line?
Well, four times X one plus three times X two equals 12,
yes, it lies on the line.
Now, let's check this point.
Zero four.
Does it satisfy the equation?
Yes, it satisfies the equation, as well.
So there's, indeed, the line,
the red line shown in the figure.
So this is in two dimensions,
what happens in D dimensional space?
What does a linear boundary look like there?
And it's a direction realization of the previous form, okay?
So when we're in D dimensional space,
then X is a vector with D components, X one through X D,
and a linear boundary,
a linear separator is something of the from
some constant W one times X one
plus some constant W two times X two,
plus all the way to some constant Wd times Xd
equals some other constancy, okay?
This is the form of a linear separator
in D dimensional space.
Now, if you look at the left hand side of that equation,
it looks a lot like a dot product, okay?
And in fact, it is...
It can just be written as W dot X equals C.
Where W is the D dimensional vector
of coefficients W one trough Wd.
So dot products allow us to express linear boundaries.
Let's see another example of this,
and then generalize a little bit, okay?
So on top over here, we have a function
that takes a four dimensional vector X one through X four,
and returns a linear function of these four features, okay?
So let's see what we have here.
We have
f of X one, X two,
X three, X four
is...
Let's go ahead and write it as a dot product, okay?
So the coefficient for X one is three.
The coefficient for X two...
There is no X two, so let's make that a zero.
The coefficient for X three is negative two,
and the coefficient for X four is zero.
So it's this dot X one,
X two, X three,
X four.
This is how we write down this linear function
using a dot product.
Now, let's look at the second example over here,
which is a little bit of a generalization.
So now, again, we take a four dimensional vector,
but this time, instead of spitting out just one number,
we are spitting out three separate numbers.
The output is a three dimensional vector,
and each of the dimensions is just a linear function of X.
Okay?
So let's see how we would write that.
So we take...
This is a function that maps
X one, X two, X three, X four
to
four
negative one,
zero, zero dot X,
so this is X over here.
The second coordinate is just X three,
so that's zero, zero, one, zero dot X.
And the third coordinate is minus one,
zero, zero, six dot X.
This is the function that we're talking about, okay?
So we can write this in a more convenient form
using matrices.
So our first row is four, negative one, zero, zero.
The second row is zero, zero, one, zero.
The third row is minus one, zero, zero, six
times X, which is X one, X two,
X three, X four.
We have expressed it as a matrix times a vector, okay?
So let's just go ahead and talk in a little bit more...
In a slightly more abstract way
about this matrix vector product.
How exactly does one multiply a matrix by a vector?
Okay, so let's say we have a matrix that's R by D,
that means that it has R rows and D columns.
So we have this matrix
and it has R rows,
let's call them M one,
M two, all the way to M of R.
So we have R rows and each row is a D dimensional vector,
so each row has length D.
We want to multi it by a vector.
The answer, in this case,
is simply the first row dot producted with the vector,
the second row dot product with the vector,
all the way to the Rth row dot product with the vector.
So we start with the matrix, that's R by D.
We multiply it by a vector, which is D by one,
it has D entries and the result is R by one.
That's the matrix vector product,
it's just a series of dot products.
Now, a matrix vector product captures a linear function,
as we've seen, and the simplest possible linear function
is just sending X to itself, the identity function.
What matrix realizes that function, okay?
That's the identity matrix.
It's a square matrix,
if the vector X is D dimensional,
it's a D by D matrix, and it has ones along the diagonal
and zero everywhere else, okay?
So if you take the identity matrix
and you multiply it by any vector X,
you get back the same vector.
Very simple linear transformation.
Now, we will sometimes be using identity matrices
in several different dimensions.
And so in those cases, we'll often use the subscript
to denote what specific size identity matrix
we're referring to, okay?
So I sub D means a D by D identity matrix.
Now let's move on to matrix-matrix products,
so multiplying one matrix by another matrix.
How do you do that, okay?
It's a very simple rule,
and again, it's built out of dot products, okay?
So we start with a matrix A,
and in this case, we have one that is R by K,
so that means it has R rows and K columns,
so let's number the rows A one through Ar
R by K.
Then, we have a matrix B, which is K by P.
That means that it has P columns.
Let's go ahead and number the columns.
Let's call them B superscript one,
all the way to B superscript P.
So this is a K by P matrix.
The result of these two is gonna be an R by P matrix.
So the result, which is A times B
is going to be an R by P matrix, okay?
And the IJ entry of that matrix,
so if you look at the entry and row number I
and column number J,
that entry over there
is A sub I
dot product with B sub J.
The IJ entry of AB is simply the dot product
of the Ith row of A with the Jth column of B, okay?
So in order to compute the product,
we simply take a bunch of dot products
of every row of A with every column of B.
Now what this means is that if you want to multiply
two matrices, the inner dimensions of the two matrices
have to agree, we need a K in both these positions.
And the product, the product matrix,
the size of that matrix is given by the outer dimensions.
So we take R by K and K by P and we get something
that's R by P.
Let's do a little example of this, okay?
So let's take
any matrix A,
maybe one, two, three, four, five, six.
Let's multiply it by some matrix B.
How about one, zero, minus one,
zero, two, one, okay?
So what are the dimensions here?
Well, this is two by three.
This is three by two.
And indeed, the inner dimensions agree, as they must.
What is the product?
What's gonna be the size of the product?
Well, it's just given by the outer dimensions.
It's gonna be two by two, so let's make space for that.
The answer is gonna be some two by two matrix,
so we have four numbers to fill in.
What are those four numbers?
Well, we take the first row of A, which is this row,
and we take the dot product with the first column of B,
so let's see what that is.
It's one minus three, so it's negative two.
What number goes in the second position?
We take the first row of A dot producted
with the second column of B.
So we get zero, four, three, we get seven.
Two more numbers to fill in.
We now move on to the second row of A.
We take the dot product with the first column of B,
so that's four minus six, which is negative two.
And the final number is
four times zero
plus five times two
plus six times one, which is 16.
So that's the product of these two matrices, very simple.
So here's the formula again, the formal expression
for the product of two matrices.
The I J entry of the product is just a dot product
between the Ith row of A and the Jth column of B.
Now there are some important properties of these products.
The first is that when you multiply something
by the identity matrix, it does not change,
that's to be expected.
The second is a rather interesting one.
So it says that
if you take the transpose of a product,
it's like taking the product of the transposes
but with the flipped order, okay?
Now, this is something which you can check
by just plugging in the definition of the product,
by just plugging in the summation you see over here
and just checking that left and right hand sides
really work out correctly.
But why don't we, at least, as a basic sanity check,
just at least check that the dimensions
of the two sides are the same, okay?
So what is the dimension of AB transpose?
Well, we've already seen that in this case,
if A is R by K and B is K by P,
then AB is R by P, so AB transpose is switching the rows
and columns, so the dimension of it is gonna be P by R.
Okay?
Now, let's look at B transpose A transpose.
B transpose has dimension
B by K
A transpose has dimension K by R.
So good, you can actually multiply them,
since these inner dimensions agree,
and the result will have dimension P by R.
So at least it's the right size.
And it turns out that these two matrices
will also be identical.
Now, for this last one, what we're being asked
is that we have these vectors U and V,
so we have U,
a D dimensional vector
and we have V, a D dimensional vector.
What is U transpose V, okay?
So let's compute the transpose of U.
So we just take that column vector
and make it into a row.
So U transpose V
is equal to
U one to Ud
multiplied by V one to Vd.
Okay, so we take each row of the first matrix
and multiply it by each column with the second matrix.
Oh, it's just the dot product of U and V.
So this is interesting.
We have two ways of writing exactly the same thing.
The dot product of two vectors U dot V
is exactly the same as U transpose V.
So this a useful fact to remember.
It's something that we'll be using to simplify
a bunch of calculations later on, okay?
So U transpose V is just a dot product between U and V.
Let's look at a couple of examples, okay?
So now let's say we have a D dimensional vector X,
so X has got D numbers.
What is X transpose X?
Well, we just saw this.
It's the dot product of X with itself.
And what's that?
That's just a squared length of X.
So X transpose X is just a number,
it's the squared length of X.
What about XX transpose?
So XX transpose, so let's see.
X is this vector.
So X is D by one.
X transpose looks like this.
It's one by D.
So the product is D by D.
It's a big matrix.
Okay.
That's a little strange.
What is the IJ entry of this matrix?
It is XiXj.
So it's the D by D matrix of all pairwise products
or features of X.
So these are also two very useful things to bear in mind.
X transpose X, versus XX transpose.
Now, they look almost the same, but as you can see,
they're completely different.
One of them is just a simple number,
the length of the vector squared,
and the other is a full D by D matrix, okay?
So one of the things this really goes to show is
that you cannot change the order
in which things are multiplied, okay?
And so this is a very general
and important property of matrices.
In general, matrix multiplication is not commutative.
AB is not the same as BA, okay?
Unless you get lucky, okay?
So let's look at these examples, for instance.
So here we have two matrices, A and B.
And let's multiply them one way
and multiply them the other way
and see if we get the same answer, okay?
They're both square matrices,
so we know they're both two by two,
and so we know the result of the two by two.
Let's see what we get in this case.
So we get one plus two, that's three.
Zero and zero is zero.
Zero and one is one.
Zero and zero is zero, okay?
So that's the first product.
The second product is one,
two.
One,
two.
They are completely different,
they aren't even close, okay?
So this is something to be a little bit careful about,
you cannot switch the order in matrix multiplication.
One thing you can do, however,
and something that's very convenient is that when
you're multiplying together a bunch of matrices,
you can decide which pair of multiplications
you're gonna do first, as long as you keep them
in the original order.
For example, you can decide,
okay, you have to multiply together ABCD.
Why don't do AB first and then do CD,
and then multiply them together?
That's allowed.
Or you can do BC first,
and then multiply the answer by A,
and multiply that answer by D and so on, okay?
So you can parenthesize the expression
in whatever way you like,
as long as you maintain the order of the matrices.
Let's look at a little example of this.
So here, let's say we have a vector X whose length is two.
What is this huge expression over here?
Okay, so clearly there are a lot of things
to be multiplied together,
but parts of it look familiar,
we've seen these sort of things before,
X transpose X, XX transpose.
What are they?
Okay, X transpose X, that's a D by D matrix, okay?
XX transpose is a D by D matrix,
X transpose X is just a number.
Which should we prefer?
The number, that seems a lot simpler.
So let's do those first, okay?
So we'll take X transpose X,
we know that's just the length of X squared.
Oh, here's another X transpose X,
that's also the length of X squared.
And here's another one and another one.
And so what we end up with
is the length of X to the power 16.
And the total length of X is two,
so this is two to the 16.
Okay?
So the associative rule can be very helpful
in simplifying matrix products, okay?
We simply choose the products
that turn out to be very simple and do those first.
So that's it for our second installment
of linear algebra.
We now have all the notation and tools we need
to be able to model linear functions,
which is something we're gonna be using
very heavily in this course.

I included some posts for reference.

https://github.com/noey2020/How-to-Talk-Linear-Algebra-Review-1

https://github.com/noey2020/How-to-Talk-2D-Generative-Modeling

https://github.com/noey2020/How-to-Talk-Probability-Review-3

https://github.com/noey2020/How-to-Talk-Probability-Review-2

https://github.com/noey2020/How-to-Talk-Generative-Modeling-in-One-Dimension

https://github.com/noey2020/How-to-Talk-Probability-Review-1

https://github.com/noey2020/How-to-Talk-Generative-Approach-to-Classification

https://github.com/noey2020/How-to-Talk-of-Fitting-a-Distribution-to-Data-

https://github.com/noey2020/How-to-Talk-of-Host-of-Prediction-Problems

https://github.com/noey2020/How-to-Talk-of-Useful-Distance-Functions

https://github.com/noey2020/How-to-Talk-of-Improving-Nearest-Neighbor

https://github.com/noey2020/How-to-Talk-of-Prediction-Problems

https://github.com/noey2020/How-to-Talk-Matlab-Tricks-and-Tweaks

https://github.com/noey2020/How-to-Talk-Trading-and-Investing

https://github.com/noey2020/How-to-Work-in-Matlab-Development-Environment

https://github.com/noey2020/How-to-Talk-Vaccines

https://github.com/noey2020/How-to-Talk-Regression-in-Matlab

https://github.com/noey2020/How-to-Get-Started-in-Matlab

https://github.com/noey2020/How-to-Convert-Data-from-Web-Service-Using-Matlab

https://github.com/noey2020/Quote-for-the-Day

https://github.com/noey2020/How-to-Talk-Good-Investment-Strategy

https://github.com/noey2020/How-to-Talk-of-Good-Plan

https://github.com/noey2020/Thought-for-the-Day

https://github.com/noey2020/How-to-Talk-Stock-Watch-of-the-Day

https://github.com/noey2020/How-to-Talk-Data-Science

https://github.com/noey2020/How-to-Talk-Fundamental-Analysis

https://github.com/noey2020/How-to-Read-Company-Profiles

https://github.com/noey2020/How-to-Import-Data-from-Spreadsheets-and-Text-Files-Matlab-Without-Coding

https://github.com/noey2020/How-to-Talk-Model-of-Stock-Market-Prices-

https://github.com/noey2020/How-to-Talk-Digital-Wallets

https://github.com/noey2020/How-to-Talk-Investing

https://github.com/noey2020/How-to-Double-Your-Money-in-5years

https://github.com/noey2020/How-to-Talk-Matlab

I appreciate comments. Shoot me an email at noel_s_cruz@yahoo.com!
