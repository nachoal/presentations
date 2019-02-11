# Reboot ♻️
> **"There is no formation without repetition"** - @wesbos

1. Introduction
2. Data types
3. Variables 
4. Methods
5. Conditionals
6. Loops
7. Iterators & blocks


## **Introduction or Don't be afraid to touch your keyboard  ⌨️**

This bootcamp is about building stuff. You won't learn programming by reading theory and trying to understand every single word in a method. You'll learn by sitting down on your terminal and using the things you learn during classes until you understand what they do. Then applying those to your problems.

### **Just in Time learning**

You came to the bootcamp to have an awesome way of learning to code so don't worry about what's not mentionted in your lectures.

You don't need to search for even more information than what you are given right now. Only search what you need to know to solve the problem you are facing.

![Martian](https://i.embed.ly/1/image?url=https%3A%2F%2Fi.imgur.com%2F8k0jFTx.jpg%3Ffb&key=522baf40bd3911e08d854040d3dc5c07)

### **Trust the program!** 


✅ Good way of learning (Active): 
1. Listen to the lecture
2. Try the concepts out on your own
4. Read all of the problem description and specs
5. **Break it down into small parts**
5. **Pseudocode it before starting**
6. **TRY TO CODE ON YOUR OWN!**

❌ Bad way of learning (Passive):
1. Don't ask if you have questions on the lecture
2. Search google for even more information about a topic before even starting a challenge.
3. Read half the challenge. 
3. Open the files and try to understand every single bit of code on your files and tests
4. ??? 


--- 


## **Data types**
```
# TEXT 
"Dwight Schrute".class              #=> String

# NUMBERS
27.class                        #=> Integer
3.14.class                      #=> Float

# GROUPINGS 
["Dwight Schrute", 27, 3.14].class  #=> Array
(1..100).class                  #=> Range

# BOOLEANS
true.class                      #=> TrueClass
false.class                     #=> FalseClass

# SPECIAL VALUES
:symbol.class                   #=> Symbol 
nil 
```
Each data type has its own methods and behaviours

--- 
## **Variables**
The object you are gonna use the most in Ruby

Store values to re-use them

```
age = 27
name = "Ignacio"
last_name = "Alonso"
favorite_emoji = "🔥"

# What's the difference between 
age = 27 
'age' == 27 

?
```
--- 

## **Methods**
Pieces of ruby code that are consicely named.
They make it easy to run code on dynamic inputs

**Without parameters:**
```
def format_date
  date = Date.today
  return date.strftime("%B %d")
end
```

**With parameters:**
```
def capitalize_your_name(name, last_name)
  return  "#{name.capitalize} #{last_name.capitalize}"
end
```

### **Arguments vs parameters**
```
def new_population(population, births)
  return population + births
end

puts new_population(2000000, 300)
```
>**Arguments are values taken by the parameters**

### Scopes

According to Wikipedia: 

> In programming, the scope of a name is the part of a program where the name is valid: where the name can be used to refer to something else. - Wikipedia

Scopes are "delimited ground areas" where the objects inside them are only visible there. 

**Example 1**
```
def add_five(number)
  return number + 5
end

puts add_five(5) #=> 10
puts number #=> undefined local variable or method 'number'
```
**Example 2**
```
first_name = 'Ignacio'

def tell_name(name)
  "You are #{first_name}"
end

tell_name(first_name) #=> undefined local variable or method `first_name' for main:Object
 ```


### Conventions 
1. Methods and variables in snake_case
2. Without return a method returns the last statement executed.
3. methods ending with a `?`
4. destructive methods ending with a `!`

--- 

## Conditionals


### **If else**
```
if (condition is true/false)
  run this code
else 
  run this code
end
```
### **Ternary operator  ` ? : `**
```
(condition true/false) ?  if true run this code : if false run this code
```
### **Multiple conditions  `if elsif else end `**
```
if (condition is true/false)
  run this code
elsif (condition is true/false)
  run this code
else 
  run this code
end
```

### **case / when / else**
```

case variable
when conditional
  run this code
when conditional_two
  run this code
else
  run this code
end
```
---

## Loops

### While (Careful with meeting your condition it could be infinite)
while  condition do
 run code
end
### Until

```
until condition do
  run code
end

```

## **Iterators & blocks**
### For (used to loop over a collection of elements)
```

for variable in array do
  run code
end
```

### **Each (used to loop over an array)**
```
emoji_cooking = ['🔥', '🐔', '🍖']

# We are iterating through our array using a one line block
emoji_cooking.each {|emoji| puts emoji}

# Multiline blocks

counter = 1

emoji_cooking.each do |emoji|
  puts "Step #{counter} #{emoji}"
  counter += 1
end
```

### **Each with index**
```
musicians = ['Ringo', 'John', 'Paul', 'George']

musicians.each_with_index do |musician, index|
  puts index.to_s + " "+ musician
end

#=> '0 Ringo'
#=> '1 John'
#=> '2 Paul'
#=> '3 George'

```
### **.map**
```
musicians = ['Ringo', 'John', 'Paul', 'George']

musicians.map! do |musician|
  musician.upcase
end


puts musicians

#=> 'RINGO'
#=> 'JOHN'
#=> 'PAUL'
#=> 'GEORGE'
```
---

## **Recommendations**


### **Accept frustration**

- You will get frustrated at all levels, but there's **always** a solution.
- If you are stuck in a problem for a long time... take a break, walk or 🍺?

### **Know your resources**

- Available data in your problem
- Take a look at the built-in methods Ruby has for you.
- You do not need to memorize all methods and how they work. It's enough to know about their existence, later you will Google them.

### **Step by step (Astronaut style 🚀)**

- What I have → What needs to be
- Data type transformation (e.g. I have **Integers** as parameters in a method, but I need to return a **String** )

### **Do a hand-written example**


### **Pseudocode**

- Descriptive steps in English. Not actual code!

### **Good orthography ⇒ Easy to read.**

- Try to indent lines
- Follow conventions
- Self-explanatory variables.
- Code is written to be read

### **Try to read code as the computer**

- Follow the flow as the computer does.
- Understand what the code is doing, line by line

### **Basic checkup**

- File saved?
- Syntax looks good?

### **Do not infere Ruby understands you**

- For Ruby all variables are value holders. Ruby does not care abou the name.

## Basic testing

- What should be the outcome?

### **Make manual testing in Terminal ≠ Rake**

- Sometimes it isn't enough just imagining or infering how the code works, always a visual feedback, a.k.a. Terminal, will make you understand better how the computer is reading the code.
- Practice in the terminal
    - `irb` for test Ruby methods.
    - `ruby` for running scripts.
- `puts` your variables when errors (step by step)

    classes, values....

### **Be open-minded when you get errors (programmers have error messages every single day)**

- You may think the code is ok, but then... ***ruby slap***

### **Google everything!**

- Methods
- Syntax
- Others solutions
- Read Ruby Docs

[Index of Files, Classes & Methods in Ruby 2.5.0 (Ruby 2.5.0)](https://ruby-doc.org/core-2.5.0/)

### **Practice!**

- Better practice than trying to memorize.