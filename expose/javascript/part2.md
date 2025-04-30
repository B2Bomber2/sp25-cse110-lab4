1. ^^^ What will happen at line 12 and why? If the code causes an error, explain why. ^^^
- it prints 3
- i is a global variable
- since the length of prices is 3, i ends up being 3

2. ^^^ What will happen at line 13 and why? If the code causes an error, explain why. ^^^
- it prints 150
- discountedPrice is a global variable
- the last discountedPrice calculation is 300 * (1 - 0.5) = 150

3. ^^^ What will happen at line 14 and why? If the code causes an error, explain why. ^^^
- it prints 150
- since finalPrice takes discountedPrice and rounds it, it produces approximately the same output as number 2

4. ^^^ What will this function return? Give a brief explanation why. If the code causes an error, explain why. ^^^
- [50, 100, 150]
- the function returns discounted 
- discounted adds the finalPrice of each input item after a discount is applied. 
- since the input is [100, 200, 300] with a discount of 0.5, the result is [50, 100, 150]

5. ^^^ What will happen at line 12 and why?  If the code causes an error, explain why. ^^^ (assume this function is being called like the others: discountPrices([100, 200, 300], 0.5)).
- There is an error
- i is declared using a let
- i is not defined outside of the for loop. 

6. ^^^ What will happen at line 13 and why? If the code causes an error, explain why. ^^^
- There is an error
- discountedPrice is declared using a let
- discountedPrice is not defined outside of the for loop. 

7. ^^^ What will happen at line 14 and why? If the code causes an error, explain why. ^^^
- it prints 150
- the finalPrice variable was declared in the same scope as line 14
- so, line 14 returns the value of the last finalPrice calculated. 

8. ^^^ What will this function return? Give a brief explanation. If the code causes an error, explain why. ^^^
- [50, 100, 150]
- the final prices are put into the discounted array.
- since the discounted array is in scope of the return function, it returns

9. ^^^ What will happen at line 11 and why? If the code causes an error, explain why. ^^^
- there is an error
- i is only defined in the for loop
- so, i is not defined in line 11

10. ^^^ What will happen at line 12 and why? If the code causes an error, explain why. ^^^
- 3 is printed
- length is declared in the same scope as line 12. 
- so, line 12 prints the value of length without errors

11. ^^^ What will this function return? Give a brief explanation. If the code causes an error, explain why. ^^^
- [50, 100, 150]
- the discountedPrice 
- discounted is in scope of the return function, so no errors are thrown. 

12. Given the above Object, write the notation for:  (These should be in your part2.md)
- Accessing the value of the name property in the student object
    - student.name

- Accessing the value of the Grad Year property in the student object
    - student["Grad Year"]

- Calling the function for the greeting property in the student object
    - student.greeting()

- Accessing the name property of the object in the Favorite Teacher property in student
    - student["Favorite Teacher"].name

- Access index zero in the array of the courseLoad property of the student object
    - student.courseLoad[0]

13. Arithmetic
- '3' + 2
    - 32
    - since 3 is a string, + becomes concatenation

- '3' - 2
    - 1
    - since it is subtraction, 3 is converted from sting to int

- 3 + null
    - 3
    - since 3 is an integer, + becomes addition
    - null becomes 0

- '3' + null
    - 3null
    - since 3 is a string, + becomes concatenation

- true + 3
    - 4
    - since it is addition, true becomes 1

- false + null
    - 0
    - since it is addition, false is 0 and null is 0

- '3' + undefined
    - 3undefined
    - since 3 is a string, + becomes concatenation

- '3' - undefined
    - NaN
    - undefined cannot become an int for subtraction

14. Comparison
- '2' > 1
    - true
    - 2 converts from string to int
- '2' < '12'
    - false
    - since they are both strings, it is a lexicographic compare
- 2 == '2'
    - true
    - the double equal allows for type changes
- 2 === '2'
    - false
    - the triple equal makes sure they are both same type and value
- true == 2
    - false
    - true becomes 1
- true === Boolean(2)
    - true
    - 2 is not 0, so the boolean version would be true
    - since both are same type and same value, it is true

15. Explain the difference between the == and === operators.
- the double equals allows type changes before comparing the values 
- in other words, the double equal only compares the values of each
- the triple equal is more strict and compares both the values and the types

16. Given the above Object, write a for...in loop that will iterate through it and print out the value of the property if the property starts with the letter r, or if the value of that property is an odd number.  (This should be in a JS file part2-question16.js)

17. If the function above is called with the following parameters modifyArray([1,2,3], doSomething), what will be the result? Briefly walk through how you arrived at that result. (This should be in your part2.md). Here we are passing in a function as a parameter, however we can also return a function from another function just as easily, you're encouraged to play around with callbacks as they are used heavily in frontend JS development. 
- [2, 4, 6]
- the function doSomething doubles its input
- modifyArray iterates through the input array and parses each element into the doSomething function
- modifyArray then stores the output of doSomething function into the new array for returning

18. The above program only prints out the time once when executed. Modify this code such that the program prints out the current time every second.  (This should be a JS file - part2-question18.js)

19. What is the output of the above code? (This should be in your part2.md)
- 1
- 4
- 3
- 2