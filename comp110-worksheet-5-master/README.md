# comp110-worksheet-5
Base repository for COMP110 worksheet 5

## Answers

a) This algorithm checks through a list, passed in the parameters of the function, and determines whether there is a duplicate (two of the same) item in within the list. The algorithm returns a 'true' boolean if the list contains a duplicate or a 'false' boolean if not.

b) The worst case running time of the algorithm is quadratic - O(n^2) - because the list checks every item against every item and no item is found to be a duplicate. This means that when one item is checked, fully, it is check agaisnt n item (where n is the size of the list); so, run this for n items and you have n * n = n^2.

c) This altered algorithm will be using j as a 'trailing' check - checking all of the previous items that i has checked (from 0 to i - 1). The algorithm still works as it is still comparing every element in the list.

d) Because of this altered algorithm, there are significantly less checks/iterations and so the algorithm runs roughly twice as fast - due to having approximately half as many iterations. There are less iterations as the same two items aren't being checked twice, as they were being previously.

e) The equation for the new algorithm is: ```y = 0.5x(0.5x - 1)``` which can otherwise be written as: ```y = 0.5x^2 - 0.5x```, hence the new algorithm is still quadratic.

f) The time complexity for Python's sort function is: O(n log(n)). Reference: [Python Wiki: Time Complexity](https://wiki.python.org/moin/TimeComplexity)

g) O(n-1). This is because the algorithm has only one for loop, which loops through every item in the list bar the first item, hence n - 1.

h) For lists that are larger than 7 items, the python Sort algorithm would perform slower, hence the algorithm is likely to run faster. This is because the python Sort function has a time complexity of O(n log(n)); and in order for the sort method to be quicker than the algorithm,  it has to be less than n - 1. Therefore, the 'log(n)' part of the sort time complexity would have to equal less than 1, as it is multipled by n. The first value in which 'n log(n)' is less than 'n - 1' is 7.


i) A programmer might choose the slower algorithm (python's in-built sort function) as it is already available to use, no extra coding is required to implement it. This saves the programmer both time and space on their project. They might only want to use the python sort if their list is small, however.

