# JavaScript 
##### Javascript Engine is responsible to run Javascript Program

1. JavaScript Code Runs inside Execution Context</br>
      * Execution Context
          Global Execution context intialized everytime js promgram runs  
          - Memory (Variable Environment)
            * Vairables
            * Functions
                - key:value </br>
                  eg:
                    varName : 10;
                    funcName :{console }
          - Code (Thread of Execution)

2. JavaScript is a synchronous single-threaded language
    * Memory Phase (Creating memory for variables and function) </br>
        - default: 
            varName is assigned as undefined 
            funcName is assigned to function code
            eg : 
              varName:undefined
              funcNaame:{...}

    * Code Execution Phase </br>
        - For each function call new Execution Context is created


3. CALL STACK (Controls order of Execution) 
    * Each Execution context created will put into stack
    * By Default Global Execution Context is already inside
    * Once all the code is executed all the context is deleted from the Stack

4. HOISTING - functions to be safely used in code before they are declared
    * Functions declared using function keyword can be accessed anywhere (before/after declaration)
    * Arrow functions acts a variable and wont copy the function code in Execution context memory
    * Arrow functions called before initializations will be undefined

5. SCOPE 
    * Accessing variable within the block.
    * Lexical Memory( In Hirarchy) - Local Memory along with Parent

6. LET & CONST 
	- Let & Const variables are stored in seperate memory space other than global memory space
	- Accessing let & const before initialization will throws an error but incase of var it prints undefined
	- Temporal Dead zone is between ,let & const are assigned with a memory space and not assigned any value to them
	- Reference Error occurs when we try to access let & const variable before initializing the value i.e variable in Temporal Dead Zone
	- var variables can be redeclared but incase of let and const variables cannot be reintialized
	
	##### Suggestions : 
		* Move all the let & const declaration to top of the program so that we can minimize window of temporal dead zone
		* Try to declare variables using const -> let -> var (worst case)


7. ERRORS
    * SyntaxError
      * Error in syntax throws syntax error </br>
        eg: misspelled keywords,duplicate declaration

    * TypeError
      * Errors occurs while the operation cannot be performed </br>
        eg:reintializing const variable with another value;

    * ReferenceError
      * Trying to access variables that we cannot access it </br>
        eg:accessing variable that was not declared,
        variable with let & const type cannot be accessed before intialization
8. Block 
	- Blocks defined between a curly braces i.e {} its used to group multiple statement
	- It is called as Compound Statement	
	- let & const are block scoped i.e cannot be accessed outside the block


	


	


	


