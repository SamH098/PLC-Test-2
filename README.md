# PLC-Test-2
a. Lexemes
- String--> Sentence : : = "char*"

-Character --> shortSen : : = 'char'

-Escape Character--> : : = escape*"|'|\|n|r|t|v|b|a*

-Whitespaces : : = <space> | <tab> | <newline> |

-Boolean ->: : = Footbool

- Comments --> : : = note*  *note
(There is no single line comment. Every comment is multilined.) 

-Int--> Nubems : : = digit+
	

	
-Letter ::= a | ... | z | A | ... | Z
-Digit ::= 0 | ... | 9 
-ReservedWord::= Begin| End | import |lookin|passIn
	Nubems | escape* | shortSen |
	Sentence | repeat | again |shorter | longer 
	rights | wrongs | printinL|Footbool|newLook

		Keywords and Identifiers

	Begin --> Marks the begining of our program 
	End -->Marks the ending of our program 
	Travel --> Goes through a given method an 
		unspecified amount of times until stopped.
	Done -->Stops travel variable.
	shortest --> Declares interger of value of 1 bytes in memory. 
	shorter --> Declares interger of value of 2 bytes in memory. 
	Nubems -->Declares interger of value of 4 bytes in memory. 
	longer --> Declares interger of value of 8 bytes in memory. 
	esc  --> This keyword is nessesary to in order to mark 	
	             the start of an escape character.
	shortSen --> Signifies a one charater string. 
	Sentence--> Signifies a multiple charater string. 
	repeat --> Use to determine the start of an incremental loop
		that is not given set parameters, similar to an if loop. 
	again --> Use to determine the start of an incremental loop
		that is given set parameters, similar to a for loop. 
	right --> used to determine when an expresion is true.
 	wrong --> used to determine when an expresion is true.
	printinL--> Print a specific staement without going in a new line.
		  Starts with quitation ends with quotations. 

-Operator ::= ( 	-> beginning of an operation, shows the order of operation 
	    ) 	->close an operation, to end the order of operation 
	   +  	-> addition operator 
	   -   	-> subtraction operator 
	   *   	->multiplication operator 
	   /   	-> division operator 
	  %    	-> modelus operator
	   <  	-> less than 
	    <= 	->less than or equal to 
	    >=  	-> greater than or equal to
	    >  	-> greater than 
	    ==  	-> asignment operator
	     !=  	->not equal to

	order of operation : : =  ( | ) | %  | + | / | *  | - |

-Delimiter ::= # | @ | $ 
	        # -->Follow the begin keyword. Mark the start of the program. 
	       @ -->At the beginning of the end keyword. Mark the end of the program.
  	        $ --> Marks the end of a print Statement
	       
		


Rules

begin -> #
# -> import 
import -> file.txt

# -> lookin
lookin -> (term)
term -> newLook 
newLook -> =
= -> (condition)
 
# -> passIn 
passIn -> variable

# -> Nubems
Nubems -> id
id -> (
( -> % 
( -> +
( -> /
( -> *
( -> -
( -> )

# -> shorter
shorter -> digits
# -> shortest
shortest -> digits
# -> longer
longer -> digits

# -> Sentence
Sentence -> string
Sentence -> digits
Sentence -> symbols

# ->  shortSen
shortSen ->  character 

# -> again
again -> nubems
id -> integer 
# -> repeat
repeat -> nubems
id -> integer

# -> printL
printL -> string 
printL -> digits
digits -> $

# -> Footbool
Footbool -> term < term
Footbool -> term <= term 
Footbool -> term >= term 
Footbool -> term > term 
Footbool -> term == term 
Footbool -> term != term 
 
#->@
@-> End


-The code is ambiguous because it did not pass ll(1) test. 

