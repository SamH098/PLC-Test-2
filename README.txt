a. Lexemes
- String--> Sentence : : = "char*"

-Character --> shortSen : : = 'char'

-Escape Character--> : : = esc*"|'|\|n|r|t|v|b|a*

-Whitespaces : : = <space> | <tab> | <newline> |

- Comments --> : : = note*  *note
(There is no single line comment. Every comment is multilined.) 

-Integer--> Nums : : = digit+
	sign : : = + | -
	signed_int : : = [sign] Integer
	real:= signed_int [fraction] [exponent]
	fraction ::= . digit+

-Program ::= (Token | Whitespace)*  	
-ID ::= Letter (Letter | Digit)*	
-Letter ::= a | ... | z | A | ... | Z
-Digit ::= 0 | ... | 9 
-ReservedWord::= Begin| End | import |
	Nums | esc | shortSen |
	Sentence | repeat | again |shorter |
	 longer | right | wrong | printinL

		use
	Begin--> Marks the begining of our program 
	End-->Marks the ending of our program 
	Travel --> Goes through a given method an 
		unspecified amount of times until stopped.
	Done-->Stops travel variable.
	Nums -->	
	esc  -->
	hortSen -->
	Sentence-->
	repeat -->
	again -->
	shorter -->
	longer -->
	right -->
 	wrong -->
	printinL-->

-Operator ::= ( | ) | + | - | * | / | % | < | <= | >= | > | == | != 
	order of operation : : =  ( | ) | %  | * | / | +  | - |

-Delimiter ::= ; | . | , | = | ( | ) | { | } | [ | ]




















































