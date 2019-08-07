# Basic Data Types

## Learning Goals

+ Ask IRB for the data type of a value
+ Define reserved word
+ Define data versus other words in a Ruby file
+ Describe what a data type is
+ Identify an Integer
+ Identify a Float
+ Identify Boolean Values
+ Identify String Values
+ Identify Symbol Values
+ Name the Scalar Data Types in Ruby

## Outline

+ Discuss pieces of a Ruby program
  + Every piece of Ruby code is either a keyword (do, end, if) - a bare word that we or some library in the language define, or data. 
  + For example, `do` is a Ruby keyword which you'll learn about later. I can't make a variable called do - this will throw an error. 
  + Likewise, if I type `dog` into IRB - this will throw an error (undefined local variable or method dog for main object) - I haven't told Ruby dog is, so it doesn't know what to do. 
  + dog is a bare word that I have to give a definition to
  + The third piece is data - these are some basic data types that we can use to write our program
+ Demo different data types next
  + Strings - good for text, can contain spaces and special characters. Show that "10" is a string - not a number   + Show concatenation and concatenate the number strings 
  + Integer
    + Whole numbers - can be positive or negative 
    + Show math - addition, subtraction, multiplication
    + Show trick with division - returns an integer
    + Show Modulo operation 
  + Float 
    + Show division here 
  + Boolean 
    + just true or false - show comparison operators
  + Symbol
    + like a string - but unique - good for data structures that you'll learn about later 

## Resources
+ https://docs.ruby-lang.org/en/2.2.0/keywords_rdoc.html
