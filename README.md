# Basic Data Types

## Learning Goals

+ Describe what "data type" means in Ruby
+ Identify data versus other words in a Ruby file
+ Identify some common ruby data types
+ Use the `.class` method to identify a data type in IRB

## Lesson

<iframe width="100%" height="720" src="https://www.youtube.com/embed/vLbU3YEna4Y?rel=0&showinfo=0" frameborder="0" allowfullscreen></iframe>

+ Hi guys, it's Ian from Flatiron School. In this video, we're going to look at some basic data types in Ruby. By the end of this video, you should be able to:
+ Describe what "data type" means in Ruby
+ Identify data from other words in a Ruby file
+ Identify some common ruby data types
+ Use the `.class` method to identify a data type in IRB
+ Let's get started. Before we talk about the different data types, let's talk about what we even mean by `data`.
+ Every single word in a Ruby file is one of three things - a Ruby keyword, a bare word, or a piece of data.
+ Ruby keywords are things like `if`and `end` - these are the basic core building blocks of the language.
+ We can view the entire list at the documentation page [here](https://docs.ruby-lang.org/en/2.2.0/keywords_rdoc.html) - as you can see, there aren't very many keywords
+ Because these are the core building blocks of the language, I can't overwrite the definition.
+ This means that I can't make a variable called `if`, because this would cause a conflict for Ruby.
+ So those are all the keywords in Ruby. Bare words are words that we can give meaning to in a Ruby application.
+ If I write `number = 100`, `number` is a bare word that I've given some meaning to - I've set that as a local variable pointed to the number 100.
+ Some bare words are actually defined by the core Ruby language itself. For example: the `puts` method is a bare word that Ruby defines. I could, if I wanted to, create a local variable called `puts` by writing `puts = "Hi"`.
+ You should never do this, because it's really confusing, but you could if you wanted to.
+ The third piece of a Ruby program are data. Data are simply some values or information that we want to be able to store in our program.
+ Data in programming can be different, and because of that, ruby has different data types. Data types let us treat different kinds of data (such as names and ages) differently from each other.
+ For example, I might want to do things with a name like combine it with another string of text, where as with a number, I might want to do some math on that number or perform some calculations.
+ Because we have different data types, we can treat those different kinds of data differently.
+ There are five basic data types that we'll look at today - strings, integers, floats, boolean, and symbols.
+ Strings are created using quotation marks and are really useful to store strings of text. This could be for any piece of text that you can imagine. If you visit your favorite web app right now, I bet you can identify some pieces of data that are represented by strings.
+ Strings can contain numbers or special characters. The below examples are all valid strings:
```ruby
"Hello"
"This is a string"
"LK9897*($%*&$#%)*#@@"
```
+ Integers are whole numbers that can be positive or negative. `42`, `0`, `-901` are all examples of Integers.
+ We can do math with these - addition using `+`, subtraction using `-`, multiplication using `*`, and division using `/`
+ One trick to know about Integer division - when doing math with Integers, Ruby will always return an Integer, which means it will return a whole number.
+ So if I do 9 / 4 - that will return 2, because this evaluates to 2, plus some remainder.
+ I can use the Modulo (`%`) operator to tell me what the remainder would be. The Module operator looks like a percent sign. `9 % 4` returns `1`, because this expression is going to be `2` plus one-fourth. So this is a weird thing when you're starting out - there are actually some cool programming tricks where this is helpful to know, but for now this is something to be aware of.
+ If you want to have a number with a decimal, you can use a Float. Floats are numbers that use a decimal point. `1.0`, `3.1415`, `-1.192` are all valid Floats.
+ We can do math the same way on Floats, but division here will return a Float as well. So `9.0 / 4.0` returns `2.25`
+ One other trick to know here about strings and numbers - what do you think this will return? `"10" + "10"`
+ This will actually return "1010". Why? Because both of those pieces of data are Strings, not numbers. Ruby actually doesn't know that they look like numbers to us. So instead of doing math addition, the `+` operator for strings just takes two strings and smashes them together. This is more useful for things like "Hello " + "Ian" if you want to combine text.
+ If we ever have a variable and we want to know what type of data it is, we can just ask it by using the `.class method`
```ruby
age = 10
```
+ So `age.class` will tell us that this is an Integer, while `10.0.class` will tell us that this is a Float.
+ Two more basic data types to be aware of - boolean data in Ruby is simply either `true` or `false`. This is really useful for conditional logic. I can compare two pieces of data using a double equals sign: `1 == 1` will return `true`, and `1 == 2` will return false.
+ We'll look more at this in a future video when we look at conditionals, but for now, just know that Ruby has boolean data types.
+ One other fun thing to look at: try to predict what the following statement will return: `"1" == 1`. Pause the video for a moment to think about the answer.
+ This actually returns false, because the first one is a string and the second one is an Integer. Ruby does not know that they look the same to us, just that they are not the same.
+ Finally, Ruby has a data type called a symbol. Symbols look like strings, but can't contain spaces and start with a colon. `:name` is an example of a symbol. Symbols are unique in Ruby, which make them nice for tracking data in data structures. You don't have to worry too much about that for right now, just know that this simple type of data is out there.
+ So that's it for this video! To recap what we learned:
+ We discussed what data type means in Ruby and why it's useful to have different data types.
+ We learned how to identify data versus other words in a Ruby file, and what those different words are.
+ We identified the five basic Ruby data types - String, Integer, Float, Boolean, and Symbol.
+ And we used the `.class` method to identify a data type in IRB so that we can tell what type of data something is.
+ Thanks so much for watching everyone, and happy coding!

## Resources
+ https://docs.ruby-lang.org/en/2.2.0/keywords_rdoc.html
