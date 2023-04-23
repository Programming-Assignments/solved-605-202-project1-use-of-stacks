Download Link: https://assignmentchef.com/product/solved-605-202-project1-use-of-stacks
<br>



Assume a Machine has a single register and six instructions       (Problem 2.3.10 from the LAT text.)

<strong><em>LD       A</em></strong><em>         </em>places the operand A in the register<em>  </em>

<strong><em>ST       A</em></strong><em>         </em>places the contents of the register into the variable A

<strong><em>AD      A</em></strong><em>         </em>adds the contents of the variable A to the register

<strong><em>SB      A</em></strong><em>         </em>subtracts the contents of the variable A from the register

<strong><em>ML      A</em></strong>         multiples the contents of the register by the variable A

<strong><em>DV      A</em></strong>         divides the contents of the register by the variable A




Write a program that accepts a postfix expression containing single letter operands and the operators +, -, *, and / and prints a sequence of instructions to evaluate the expression and leaves the result in the register. Use variables of the form <em>TEMPn</em> as temporary variables. For example, using the postfix expression ABC*+DE-/ should print the following:




<strong><em>LD       B </em></strong>

<strong><em>ML      C </em></strong>

<strong><em>ST       TEMP1 </em></strong>

<strong><em>LD       A </em></strong>

<strong><em>AD      TEMP1 </em></strong>

<strong><em>ST       TEMP2 </em></strong>

<strong><em>LD       D </em></strong>

<strong><em>SB      E </em></strong>

<strong><em>ST       TEMP3 </em></strong>

<strong><em>LD       TEMP2 </em></strong>

<strong><em>DV      TEMP3 </em></strong>

<strong><em>ST       TEMP4 </em></strong>

<strong> </strong>

Use the following postfix expressions for input

<strong> </strong>

<strong>AB+C-                                                                        ABC+/CBA*+ </strong>

<strong>ABC+-                                                                        AB-*CBA+-* </strong>

<strong>AB-C+DEF-+$                                                          ABC-/BA-+/  </strong>

<strong>ABCDE-+$*EF*-                                                       ABC+$CBA-+*          </strong>

<strong>ABC+*CBA-+*                                                          AB0+/CBA+-/ </strong>

<strong>             </strong>

Keep in mind that you are NOT evaluating the postfix expression, you are generating the machine language instructions that would perform the evaluation if actually executed.




In your analysis, be sure to discuss the implementation you choose and why, why a stack makes sense.  Consider a recursive solution (you do not need to implement recursion) and compare it to your iterative solution. Is one better than the other? Why? Tell us what you learned and what you would do differently. Be sure to review the programming assignment guidelines, including the formatting requirements for the analysis. You may not use library functions. You must write your own code, in particular you must write the stack code.  Be sure to include the stack source code  in your suibmission. You must read and write from named files.