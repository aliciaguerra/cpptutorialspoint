When we consider a C++ program, it can be defined as a collection of objects that communicate
via incoking each other's methods.

-  Object - Objects have states and behaviors. Example: a dog has states - color, name, breed, as
    well as behaviors - wagging, barking, eating. An object is an instance of a class.
-  Class - A class can be defined as a template/blueprint that describes the behaviors/states that
   objects of its type support.
- Methods - A method is basically a behavior. A class can contain many methods. It is in methods
where the logics are written, data is manipulated, and all the actions are executed.
- Instance variables - Each variable has its unique set of instance variables. An object's state is created
by the values assigned to these instance variables.

#C++ Program Structure

           #include <iostream>
           using namespace std;
           
           //main() is where the program execution begins
           int main()
           {
            cout << "Hello World"; //prints Hello World
            return 0;
           }
           
Let us look at various parts of the above program:

- The C++ language defines several headers, which contain information that is either necessary or useful
to the program. For this program, the header <iostream> is needed.
- The line using namespace std; tells the compiler to use the std namespace. Namespaces are a relatively
recent addition to C++. 
- The line int main() is where the program execution begins
- The next line cout << "This is my first cpp program."; causes the message "This is my first cpp program"
to be displayed on the screen
- The next line return 0; terminates main() function and causes the return the value 0 to the calling
process.

#Semicolons & Blocks in C++
In C++ the semicolon is a statement terminator. That is, each individual statement must be ended with a semicolon.
It indicates the end of one logical entity.

For example, following are the different statements:

       x=y;
       y=y+1;
       add(x,y);
       
A block is a set of logically connected statements that are surrounded by opening and closing
braces. 

       {
        cout << "Hello World"; //print Hello World
        return 0;
       }
       
C++ does not recognize the end of the line as a terminator. For this reason, it does not matter where
on a line you put in a statement.

         x=y;
         y=y+1;
         add(x,y);
         
is the same as

        x=y; y=y+1; add(x,y);
        
#C++ Identifiers
A C++ identifier is a name used to identify a variable, function, class, module, or any other
user-defined term. A identifier starts with a letter A to Z or a to z to underscore (_) followed
by zero or more letters, underscores, and digits (0 to 9).

C++ does not allow punctuation characters such as @, $, and % within identifiers. C++ is a 
case-sensitive programming language. Thus, manpower and Manpower are two different identifiers in C++.

#C++ Keywords
The following list shows the reserved words in C++. These reserved words may not be used as a constant
or variable or any other identifier names.

          asm
          auto
          bool
          break
          case
          catch
          char
          class
          const
          const_class
          continue
          default
          delete
          do
          double
          dynamic_cast
          else
          enum
          explicit
          export
          extern
          false
          float
          for
          friend
          goto
          if
          inline
          int
          long
          mutable
          namespace
          new
          operator
          private
          protected
          public
          register
          reinterpret_cast
          return
          short
          signed
          sizeof
          static
          static_cast
          struct
          switch
          template
          this
          throw
          true
          try
          typedef
          typeid
          typename
          union
          unsigned
          using
          virtual
          void
          volatile
          wchar_t
          while
          
#Trigraphs
A few characters have an alternative representation, called a trigraph sequence. A trigraph is
a three-character sequence that represents a single character and the sequence always starts with
two question marks.

Trigraphs are exapnded anywhere they appear, including within string literals and character literals,
in comments, and in preprocessor directives.

Trigraphs are exapnded anywhere they appear, including within string literals and character literals,
in comments, and preprocessor directives.

Trigraph                 Replacement
??=                      #
??/                      \
??'                      ^
??(                      [
??)                      ]
??!                      |
??<                      {
??>                      }
??-                      ~

All the compilers do not support trigraphs and they are not advised to be used because of their
confusing nature.

#Whitespace in C++
A line containing only whitespace, possibly with a comment, is known as a blank line, and C++ compiler
totally ignores it.

Whitespace is the term used in C++ to describe blanks, tabs, newline characters, and comments. Whitespace
separates one part of the statement from another and enables the compiler to identify where one element in a 
statement, suhc as int, ends and the next element begins. Therefore, in the statement

            int age;
            
there must be at least one whitespace character (usually a space) between int and age for the compiler to be able to
distinguish them. On the other hand, in the statement,
      
      fruit = apples + oranges; //Get the total fruit
      
no whitespace characters are necessary between fruit and =, or between = and apples, although you are free to include
some if you wish for readibility purpose.
          
