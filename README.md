# Automatic table generator for java programs in IN3030/IN4330  
The purpose of this script is to run any number of java programs through several iterations and generate timing tables based on median values.  
The tables will be put in a csv file called report.csv

**Usage:** python3 java\_median\_timer -j ... -n ...  

**Arguments:**  
\-j[ava]        ...     : Required argument. Specifies which java programs to generate tables for.  
\-a[rguments]   ...     : Required argument. A list of strings that specifies which arguments the java programs should be run with.

**Example:**  
python3 java\_median\_timer -j multicore singe\_core -n "10000 20" "100000 20"  
This will generate timing tables for the java executables multicore and single\_core. Each java executable is first run with the arguments 10000 20 and then with 100000 20.

**Future funcionality:**  
Add -o to allow user to specify output file    
Generate more tables
