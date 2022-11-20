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

		Keywords and Identifiers

	Begin --> Marks the begining of our program 
	End -->Marks the ending of our program 
	Travel --> Goes through a given method an 
		unspecified amount of times until stopped.
	Done -->Stops travel variable.
	shortest --> Declares interger of value of 1 bytes in memory. 
	shorter --> Declares interger of value of 2 bytes in memory. 
	Nums -->	Declares interger of value of 4 bytes in memory. 
	longer --> Declares interger of value of 8 bytes in memory. 
	esc  --> This keyword is nessesary to in order to mark 	
	             the start of an escape character.
	shortSen --> Signifies a one charater string. 
	Sentence--> Signifies a multiple charater string. 
	repeat --> Use to determine the start of an incremental loop
		that is not given set parameters, similar to a while loop. 
	again --> Use to determine the start of an incremental loop
		that is given set parameters, similar to a for loop. 
	right --> used to determine when an expresion is true.
 	wrong --> used to determine when an expresion is true.
	printinL--> Print a specific staement without going in a new line. 

-Operator ::= ( | ) | + | - | * | / | % | < | <= | >= | > | == | != 
	order of operation : : =  ( | ) | %  | * | / | +  | - |

-Delimiter ::= # | @ | $ | = | ( | ) | | [ | ]
	        # -->Follow the begin keyword. Mark the start of the program. 
	       @ -->Follow the begin keyword. Mark the en of the program.
  	        $ 
	        = 
	        ( 
 	        )   
      	       [ 
	       ]
		

