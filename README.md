# Infix-to-Postfix
Implement conversion of infix to postfix using stack

Algorithm 

Start 

Push “(“onto Stack, and add “)” to the end of X. 

Scan X from left to right and repeat Step 3 to 6 for each element of X until the Stack is empty. 

If an operand is encountered, add it to Y. 

If a left parenthesis is encountered, push it onto Stack. 

If an operator is encountered ,then: 

Repeatedly pop from Stack and add to Y each operator (on the top of Stack) which has the same precedence as or higher precedence than operator.

Add operator to Stack. 

[End of If]

If a right parenthesis is encountered ,then:

Repeatedly pop from Stack and add to Y each operator (on the top of Stack) until a left parenthesis is encountered.

Remove the left Parenthesis.

[End of If]

[End of If]

Stop
