# Algorithms-in-javascript

This project comes from my need to grow as a front-end developer studying algorithms and data structures.  
Reading this book: **Grokking Algorithms(https://amzn.eu/d/iuBzNhW)**, I'd like to do exercises related to every topic and share them with the community.  

I suggest you to buy this book if you want to have a good understanding of Algorithms and Data structures. The author provides clear explanations and very understandable examples.

Feel free to open PR if something needs to be corrected or if you want to contribute.


---
## Binary search [DRAFT]

The binary search algorithm is very useful and powerful when you have to search for an element in a **sorted list**.  

Imagine that you have a sorted array like this ```const sortedArray = [1,2,3,4,5,...,220,...,1000]```, if you're looking for the number ```220``` and you want to know its position, a common way could be to iterate the entire array with a loop, starting from ```0``` to ```array.length```, but this method/approach is very expensive if the array has two billion elements 😜.

So, in this case, we can use the ***binary search*** to improve our code. Instead of starting from ```0``` you can start your search from the middle of the array and if the number is too low (or too high) than your number, you've just eliminated half the numbers!  

Ex: the ```sortedArray``` contains 1000 numbers (from 1 to 1000), if you start from the middle you get `500`, so, since ```500``` is greater than ```220``` you've just eliminated all the numbers between ```500``` and ```1000```.  
In the next iteration you can continue with the range ```0 - 250``` looking for the position ```125```
