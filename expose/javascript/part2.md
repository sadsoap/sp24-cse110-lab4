# Expose
*****
## Part 2
#### var declaration
1. `3` is printed by line 12, since the `for` loop is iterated by the number of elements in the `prices` array passed into the `discountPrices` function. There is no error here. 
2. 150 is printed by line 13, since the final element of `prices` is `300`, and the discount is `0.5`, so the most recent assigned value to `discountedPrice` is 
`300 * ( 1 - 0.5)` = 150.
3. `150` is printed by line 14, since  `finalPrice` is not an array variable, and thus will only store the final (rounded) discounted price of the `prices` array.
4. `[ 50, 100, 150 ]` will be returned by the function. Each element is discounted in the `for` loop by 50% (or `0.5`), so the final array of prices is halved. 

#### let declaration
5. There is an error at line 12, since `i` is only defined in the scope of the `for` loop.
6. There is an error at line 13, since `discountedPrice` is only defined in the scope of the `for` loop.
7. `150` is printed by line 14, since the last assigned values/calculations done inside the `for` loop are based on the last element of the `prices` array, and `finalPrice` is defined and called inside the `discountPrices` function, but *outside* the `for` loop.
8. `[ 50, 100, 150 ]` is returned by the function. It functions the same as it did when each variable was declared/defined with `var`, since each `let` variable here is defined and used within its respective scope. 

#### const declaration & let iterator
9.  There is an error, since `i` is not defined outside of the scope of the `for` loop. 
10.  `3` is printed by line 12, since the length of the `prices` array is `3`.
11. `[ 50, 100, 150 ]` is returned by the function. It functions the same as it did with the previous variable types, since each variable here is defined and used within its respective scope. 