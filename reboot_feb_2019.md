# Reboot ♻️
> **"There is no formation without repetition"** - Wesbos

1. Introduction
2. Built in Objects 
3. Variables 
4. Methods

## **Introduction or Don't be afraid to touch your keyboard ⌨️**

This bootcamp is about building stuff. You won't learn programming by reading theory and trying to understand every single word in a method. You'll learn by sitting down on your terminal and using the things you learn during classes until you understand what they do. Then applying those to your problems.

### **Just in Time learning**

You came to the bootcamp to have an awesome way of learning to code so don't worry about what's not mentionted in your lectures.

You don't need to search for even more information than what you are given right now. 


### **Trust lewagon's program** 

![Martian](https://i.embed.ly/1/image?url=https%3A%2F%2Fi.imgur.com%2F8k0jFTx.jpg%3Ffb&key=522baf40bd3911e08d854040d3dc5c07)

✅ Good way of learning (Active): 
1. Listen to the lecture
2. Try the concepts out on your own
4. Read all of the problem description and specs
5. **Break it down into small parts**
5. **Pseudocode it before starting**
6. **TRY TO CODE ON YOUR OWN!**

❌ Bad way of learning (Passive):
1. Listen to the lecture 
2. Search google for even more information
3. Read half the problem
3. Open the files and try to understand ALL of them
4. ??? 


--- 


## **Data types**
```
# TEXT 
"Sponge Bob".class              #=> String

# NUMBERS
12.class                        #=> Integer
3.14.class                      #=> Float

# GROUPINGS 
["Sponge Bob", 12, 3.14].class  #=> Array
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
name = Ignacio
last_name = Alonso

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

### Conventions 
1. Methods and variables in snake_case
2. Without return a method returns the last statement executed.
3. methods ending with a `?`
4. destructive methods ending with a `!`

--- 

## Conditionals


### If else
```
if (condition is true/false)
  run this code
else 
  run this code
end
```
### Ternary operator  ` ? :` 
```
(condition true/false) ?  if true run this code : if false run this code
```
### Multiple conditions  `if elsif else end` 
```
if (condition is true/false)
  run this code
elsif (condition is true/false)
  run this code
else 
  run this code
end
```