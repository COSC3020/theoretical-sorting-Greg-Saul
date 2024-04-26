[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/9YUeXH71)
# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

## My Analysis

To test the claim, I would use many different possible arrays such as: empty, sorted, reverse sorted, random, and partially sorted

I would use these different arrays and use different lengths of each of them. I would use timing code to run the sorting algorithm with the different arrays then probably put the results into an excel spreadsheet and use that to graph the results. I would expect the time to grow in a linear way as the elements in the array grow. because of this, I would expect the datapoints to fall on the line of best fit that has a y=mx+b format. This would prove that as the elements got bigger, so does the time at the same rate. In order to account for inconsistencies like we learned about in a previous project, I would use the same computer for every test and I would have no background apps running if possible. 

We know from what we have learned that the best theoretical sorting time is $\Omega(nlogn)$ for comparison based sorting algorithms. This is because we only compare 2 elements at a time as described by the model that uses a binary tree where leaves are the elements of the array and the other nodes are "choice points" where comparisons are done.

These methods of testing and known limits of comparative sorting can tell us with almost certainty that the researcher is wrong about his claims of having a complexity of $O(n)$.















