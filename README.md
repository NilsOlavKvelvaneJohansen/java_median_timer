# Automatic table generator for java programs in IN3030/IN4330  
The purpose of this script is to run any number of java programs through several iterations and generate timing tables based on median values.  

**Usage:** python3 java\_median\_timer -j ... -n ...  

**Arguments:**  
\-j[ava]        ...     : Required argument. Specifies which java programs to generate tables for.  
\-n[umber]      ...     : Required argument. A list of numbers that specifies which arguments the java programs should be run with. Each of the values are timed and corresponds with the values in the x axis of the generated tables.  

**Example:**  
python3 java\_median\_timer -j multicore singe\_core -n 10000 100000 1000000 10000000  
This will generate timing tables for the java executables multicore and single\_core where the values in the x axis is 10 000, 100 000, 1 000 000 and 10 000 000.  
