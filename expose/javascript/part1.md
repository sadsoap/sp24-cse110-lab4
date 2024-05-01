# Expose
*****
## Part 1
#### var declaration
1. "values added: 20" is printed by line 9. There is an error here, if the intent is to show "10 + 10" or "10, 10". However, this is a developer/user error, not the program.
2. "values added: 20" is printed by line 13. There is no error here. 

#### let declaration
3. "values added: 20" is printed by line 9. There is no error here. 
4. This returns an error, because `result` does not exist/isn't defined outside of the `if(add)` block.

#### const declaration
5. Nothing prints here. There is an error prior, on line 7. Using `const` variables means that the variable cannot be changed once defined, so there is an error when we try to assign a new value to it.
6. Nothing prints here, for the same reason as above. The program stops after the previous error. Should line 7 be removed or commented out, line 13 still would not print, as `result` would not be defined outside of the `if(add)` block, similar to `let`.