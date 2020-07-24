# Python-Parser
Recursive descent parser in Python 3 based on the grammar:<br />
Provided is a predictive BNF grammar for the boolean expressions: <br />
any boolean variable is a boolean expression, any boolean constant True and False is a boolean expression. <br />
If expr1 and expr2 are two boolean expressions, so are expr1 and expr2 and expr1 or expr2 and not expr1. <br />
Grammar is designed so that the operators and and or have the same level of precedence and are left associative, <br />
while the unary operator not is right associative and has a higher level of precedence than and and or . <br />
The assignment expression is also a boolean expression and has the form var = expr where var is a name of a boolean variable and expr is a boolean expression, <br />
The operator = should be right associative and its level of precedence should be the lowest, <br />
thus var = expr1 or expr2 should have the meaning of var = (expr1 or expr2) <br />
