# implement List.indexOf

`while`-style and recursive implementations at the top of
OrderedList_inArraySlots.java

[Java API on the `indexOf` method](https://docs.oracle.com/javase/10/docs/api/java/util/List.html#indexOf(java.lang.Object))

based on [solutionsHolmes/5D_genericTypes/OrderedList_inArraySlots_v2/](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/5D_genericTypes/OrderedList_inArraySlots_v2)
as of 2019-04-10 04:48


# Recall inverse functions and logarithms
**What is meant by y = log<sub>2</sub>x?
The value of "y" is the exponent to raise 2 to in order to obtain the value of "x"

** What does its graph look like?
The graph looks like a reflection of y = 2<sup>x</sup> across the line y = x.

# Describe the recursive solution
0. State the problem
Find the index of an element in an ordered list.
1. State the recursive abstraction
When asked to find the index of an element in an ordered list,
the recursive abstraction can find the index of the elemnent
in one-half of the ordered list.
2. Identify the parts of this solution that correspond to the six parts of a generalized recursive solution:

- binary statement:
	if (low > hi) // detect base case 0
	if (comparison == 0) // detect base case 1

- instructions to solve the base case"
	return -2; // solution to base case 0
	return pageToCheck; // solution to base case 1

- instruction to solve the recusive case
	* combination process
		- n/a
	* leftover processing
		- n/a
	* result of the recursive abstraction
		return indexOf_recursive( findMe
								, low
								, pageToCheck - 1);

