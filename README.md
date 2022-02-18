# Automatic table generator for java programs
The purpose of this script is to run any number of java programs through several iterations and generate timing tables based on median values.  
For this script to work you will need to ensure that your java program runs the part you want to time seven times and prints the time taken every iteration. This is to ensure that the JIT compiler will take effect.  
Results will be output in a file called results.xlsx  
  
**Dependencies:**  
Numpy: install with ```pip install numpy```  
Pandas: install with ```pip install pandas```
Openpyxl: install with ```pip install openpyxl```
  
**Usage:**  
python3 java\_median\_timer -j ... -a ...  
  
**Arguments:**  
\-j[ava]        ...     : Required argument. Specifies which java programs to generate tables for.  
\-a[rguments]   ...     : Required argument. A list of strings that specifies which arguments the java programs should be run with.
  
**Example:**  
python3 java\_median\_timer -j multi\_core singe\_core -a "10000 20" "100000 20"  
This will generate timing tables for the java executables multi\_core and single\_core. Each java executable is first run with the arguments 10000 20 and then with 100000 20.
  
**Future funcionality:**  
- Add -o to allow user to specify output file    
- Generate more tables
