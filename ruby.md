# ASSESSMENT 4: INTRO TO RUBY
## Interview Practice Questions

Answer the following questions. First, without external resources. Challenge yourself to answer from memory. Then, research the question to expand on your answer. Even if you feel you have answered the question completely on your own there is always something more to learn.   

1. In what ways are JavaScript and Ruby similar? In what ways are they different?

  Your answer: Similar: Scripting languages, object oriented, dynamic language, use framwork in both(React, Rails)
               Differences: JS optimized for Browser, speed doing certain task, JS has const, let,var. 

  Researched answer: JavaScript and Ruby are object-oriented, dynamic and general purpose scripting language which is interpreted rather than compile during runtime. JavaScript can be used as front-end and back-end language using the same language whereas Ruby is used as back-end programming language.



2. What is a hash?

  Your answer: Collection of key value pairs, used for storing collection of grouped information, represent objects.
  bie={
    number_of_tires:2
    number_of_inflated tires:1
  }

  Researched answer:
A Hash is a collection of key-value pairs like this: "employee" = > "salary". It is similar to an Array, except that indexing is done via arbitrary keys of any object type, not an integer index.





3. What is the testing framework used in Ruby? Describe the process of setting up the testing environment.

  Your answer: rspec.

  Researched answer: gem install rspec
  (in Rails)
  rails new BIkeTireBlowout -T (the -T means no testing, so we can add our own)
  gem install rspec-rails
  Rails generate rspec:install



4. Name three possible relationships between objects?

  Your answer:
  has_many
  belongs_to
  is_a

  Researched answer: has_one,has_many,has_many:through,  belongs_to, is_a 
   class Body
   has_many:hands
   end
   class Hand
   has_many:fingers
   end
   class Finger
   belongs_to:hands
   end
                      




5. What is an instance variable? How is it different from other variables in Ruby?

  Your answer: has a name begining with @

  Researched answer: An instance variable has a name beginning with @, and its scope is confined to whatever object self refers to. Two different objects, even if they belong to the same class, are allowed to have different values for their instance variables. From outside the object, instance variables cannot be altered or even observed (i.e., ruby's instance variables are never public) except by whatever methods are explicitly provided by the programmer. As with globals, instance variables have the nil value until they are initialized.



6. Ruby has a great community and tons of free resources to help you learn. [Here](https://www.ruby-lang.org/en/documentation/)is a list of great resources. Below are a few popular ones:
- [Interactive Ruby Tutorial](http://tryruby.org/levels/1/challenges/0)
- [Why's (poigniant) Guide to Ruby](http://poignant.guide/book/chapter-1.html): comics, anecdotes, and microscopic canaries
- [Ruby in 20 Min](https://www.ruby-lang.org/en/documentation/quickstart/)
- [Ruby Style Guide](https://rubystyle.guide/)

Choose one of these resources and look through the material for 10-15 min. List three new things you learned about Ruby:

1). Been around since 1991

2).Symbols are elegant, and beautiful

3). Comment on the first line indicated to shel instructions. Use Ruby interpreter for example or linting

4).__FILE__ ferers to file is it execute in

5). Array comparison is off the chain [1,2,3] | [1,4]=[1,2,3,4]


7. STRETCH: What are blocks, procs, and lambdas?

  Your answer: 
  do 
  puts "this is a block"
  end
  {
    puts "this is also a block"
  }
  lambda:
  ->(input){puts "this is a lambda"}
  
  
  
  
  

  Researched answer: In Ruby, blocks are snippets of code that can be created to be executed later. 
  Blocks are passed to methods that yield them within the do and end keywords. 
  One of the many examples is the #each method, which loops over enumerable objects.
  A “proc” is an instance of the Proc class, which holds a code block to be executed, and can be stored in a variable. 
  To create a proc, you call Proc.new and pass it a block.
  Lambdas are essentially procs with some distinguishing factors. They are more like “regular” methods in two ways: 
  they enforce the number of arguments passed when they’re called and they use “normal” returns.
  
  
