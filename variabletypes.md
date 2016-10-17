A variable provides us with named storage that our programs can manipulate. Each variable
in C++ has a specific type, which determines the size and layout of the variable's memory;
the range of values that can be stored within that memory; and the set of operations that cen be applied
to the variable.

The name of a variable can be composed of letters, digits, and the underscore character. It must begin 
with either a letter or an underscore. Upper and lowercase letters are distinct because C++
is case-sensitive.

bool    Stores either value true or false.
char    Typically a single octet (byte). This is the integer type.
int     The most natural size of the integer for the machine.
float   A single-precision floating point value.
double  A double-precision floating point value
void    Represents the absence of type
wchar_t A wide character type.

C++ also allows to define various other types of variables, which we will cover in subsequent chapters like
Enumerations, Pointer, Array, Reference, Data Structures, and Classes.

#Variable Definition in C++
A variable definition means to tell the compiler where and how much to create the storage for the variable. 
A variable definition specifies a data type, and contains a list of one or more variables of that type as follows:

              type variable_list;
              
Here, type must be a valid C++ data type including char, w_char, int, float, double, bool, or any user-defined object
and variable_list may consist of one or more identifier names and separated by commas. Some valid declarations are shown here:

              int i, j, k;
              char c, ch;
              float f, salary;
              double d;
              
 The line int i, j, k; both declares and defines the variables i, j, and k; which instructs the compiler to create
 variables named i, j, and k of type int.
 
 Variables can be initialized (assigned an initial value) in their declaration. The initializer consists of an equal sign
 followed by a constant expression as follows:
 
               type variable_name = value;
               
 Some examples are:
 
              extern int d=3, f=5; //declaration of d and f
              int d=3, f=5; //definition and initializing d and f
              byte z = 22; //definition and initializes z
              char x = 'x'; //the variable x has value 'x'
              
 For defintiion without an initializer: variables with static storage duration are implicitly initialized 
 with NULL (all bytes have the value 0); the initial value of all other values is undefined.
 
 #Variable Declaration in C++
 A variable declaration provides assurance to the compiler that there is one variable existing with
 the given type and name that the compiler proveed for further compilation without needing complete detail about the variable.
 A variable declaration has its meaning at the time of compilation only, compiler needs actual variable definition
 at the time of linking of the program.
 
 A variable declaration is useful when you are using multiple files and you define your variable in one of the 
 files which will be available at the time of linking of the program. You will use extern keyword to declare
 a variable at any place. Though, you can declare a variable multiple times in your C++ program, but it can be defined
 only once in a file, a function, or block of code.
