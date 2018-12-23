## Documentation
This directory presents MATLAB coded solutions to questions from [Euler Project](https://projecteuler.net/).
The code can be directly downloaded and run to obtain the answer. Solutions to questions on Euler Project can be found in many different ways, therefore, it should not be a shock to see a completely different approach that is attempted here and yet returns the right answer. So far 10 questions are solved, but the directory will continue to get updated as more solutions are uploaded. The name for each piece of code for a particular question is self explanatory in the format of the word 'EuPr' followed by a number that corresponds to the number of question in the [Euler Project](https://projecteuler.net/) website.
### `EuPr1.m`
`Question 1: If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23. Find the sum of all the multiples of 3 or 5 below 1000.`

Solution: Construct a vector of all numbers less than 1000 that are multiples of 3 and denote it by `A=3:3:999;`, then construct another vector of all numbers less than 1000 that are multiples of 5 and denote it by `B=5:5:999;`. Define a third vector `C=union(A,B);` as the union of `A` and `B`. The answer is the sum of all elements in `C`, which is returned by `Answer = sum(C)`. 
