1. Line 12 prints 3. The variable i was declared using 'var' and so is accessible outside of the for loop. The value of i is 3 because prices.length is 3, so the for loop terminates when i >= 3. 
2. Line 13 prints 150. The variable discountedPrice was declared using 'var' and so is accessible outside of the for loop. The value of discountedPrice when the loop terminates is prices[2] * (1 - discount), or 300 * 0.5 = 150. 
3. Line 14 prints 150. The variable finalPrice was declared using 'var' and so is accessible outside of the for loop. The value of finalPrice when the loop terminates is discountedPrice, 150 as shown in question 2, multiplied and divided by 100 (the rounding does nothing in this case). 
4. This function returns the array [50, 100, 150]. After each iteration of the for loop, the finalPrice for the input at that index is pushed to the array. In this case, each finalPrice is half of the input price (since discount is 0.5), so inputting [100, 200, 300] returns [50, 100, 150]. 
5. Line 12 returns an error. The variable i was defined using 'let' inside the for loop, so since the log statement is outside of its scope, the log returns an error. 
6. Line 13 returns an error. The variable discountedPrice was defined using 'let' inside the for loop, so since the log statement is outside of its scope, the log returns an error. 
7. Line 14 prints 150. The variable finalPrice was defined at the top of the function using 'let' and so is accesible by the log statement. The value of finalPrice is 150 as shown in question 3. 
8. The function returns [50, 100, 150] as shown in question 4. 
9. Line 11 returns an error for the same reason as question 5. 
10. Line 12 prints 3. The variable length is defined using 'const' at the top of the function and so is accessible by the log statement. The value of length is 3 since the input array has 3 values. 
11. The function returns the array [50, 100, 150]. After each iteration of the for loop, the discountedPrice for the input at that index is pushed to the array. In this case, each discountedPrice is half of the input price (since discount is 0.5), so inputting [100, 200, 300] returns [50, 100, 150]. Although discountedPrice is defined using 'const', the loop is redeclaring the value rather than reassigning it, so no errors are thrown. 

12A. student.name

12B. student['Grad Year']

12C. student.greeting()

12D. student['Favorite Teacher'].name

12E. student.courseLoad[0]

13A. '3' + 2: '32'. '3' is a string, so '+' is overridden as string concatenation and 2 maps to '2', giving the string '32'. 

13B. '3' - 2: 1. There is no string operation for '-', so '3' maps to 3 and '-' performs subtraction, and 3-2=1. 

13C. 3 + null: 3. 3 is an integer, so '+' performs addition and null maps to 0, so 3+0=3. 

13D. '3' + null: '3null'. '3' is a string, so '+' is overridden as string concatenation and null maps to 'null', giving the string '3null'. 

13E. true + 3: 4. 3 is an integer, so '+' performs addition and true maps to 1, so 1+3=4. 

13F. false + null: 0. '+' performs addition and both false and null map to 0, so 0+0=0. 

13G. '3' + undefined: '3undefined'. '3' is a string, so '+' is overridden as string concatenation and undefined maps to 'undefined', giving the string '3undefined'. 

13H. '3' - undefined: NaN. '-' performs subtraction and performing mathematical operations on undefined gives NaN. 

14A. '2' > 1: true. '2' becomes the number 2, and 2 > 1 is true. 

14B. '2' < '12': false. '2' is lexicographically greater than '1'. 

14C. 2 == '2': true. '2' maps to 2 and 2 == 2 is true. 

14D. 2 === '2': false. 2 and '2' are different types, so === is automatically false. 

14E. true == 2: false. true maps to 1 and 1 == 2 is false. 

14F. true === Boolean(2): true. Boolean(2) converts to true, and true === true is true. 

15. The == operator is not strict and automatically converts values to thes ame type if possible. The === operator is strict and does not automatically convert values. 
16. (see part2-question16.js)
17. Output: [2, 4, 6]. The function takes an array and, for each item in the array, runs it through the doSomething function. In this case, doSomething multiplies the input numnber by 2, which is then stored at the original index in the array. In short, this sequence multiplies each item by 2 and returns the new array. 
18. (see part2-question18.js)
19. Output:\
    1\
    4\
    3\
    2\
    1, 4, and 3 are printed almost immediately and 2 is printed after a pause. 