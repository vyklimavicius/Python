- Python 

Differences between v2 and v3

Anaconda => The open-source Anaconda Distribution is the easiest way to perform Python/R data science and machine learning on Linux, Windows, and Mac OS X. 

- Data types:

int => whole number 
float => decimal points
str => string 
 
 ** Data structures:

 Lists, list => Ordered sequence of objects [10, "hello", 0.2] // other languages Array
 Dictionaries, dict => Unordered Key: Value pairs {"myKey" : "value"} // other languages Hashes, Objects(js)
 Tuples, tup => Ordered immutable sequence of objects (10,"hello",1.2) 
 Sets, set => Unordered collection of unique objects {"a","b"} 
 Booleans, bool => Boolean value True or False

- Create variables and use the assignment operator:

 Python variables are dynamic typed

 ex: 
 a = 5

 Variables need to be defined. If you just want a placeholder you can assign None to it.
 Ex:

 a = None

- Strings:

 * indexing : 
 string[]

 * slice:
 string[star:end] # the end position is not taken, it just means up to but do not include the word.
 string[::] # this means all the way to the beginning and ending
 string[::stepsize] # the third argument is the stepsize, means that it would jump the number of characters pass as an argument and grab the other chars.

 * A python trick to reverse a string:
 string[::-1] # this means it will go al the way starting in the stepsize last char.

 ** Note : In python strings are immutable(Python doesn't support item assignment), meaning that you cannot change a char in a string by doing this:
 string[1] = a THIS WON'T WORK.

 Are strings mutable?

 Strings are not mutable! (meaning you can't use indexing to change individual elements of a string)

 A way to do this is by using STRING CONCATENATION(remember you can't concatenate numbers with strings), EX:
 'P' + any_variable (Of course to replace first you would have to slice the older string to grab the chars you need)
 
 example:

 st = "Vytautas"
 print(st)
 new_st = st[1:]
 print(new_st)
 new_st = 'R' + new_st
 print(new_st)

 * repeating chars(times) :

 syntax:
 string * <number> 
 #=> the string repeated number of times.

 * Methods: 

 a. upper() => Uppercase collection of chars. 
 b. lower() => Lower collection of chars.
 c. split() => Creates a quick list out of the collection of chars. the split is based on the argument pass to the method.

 * String Interpolation:

 Remember, in Python Strings are not mutable! (meaning you can't use indexing to change individual elements of a string).

 Formatting with the .format() method:

 'String here {} then also {}.'.format('something1','something2'). 

 also 

 f (formatted string literals) 

 Ex:

 st = "Vytautas"

 print(st + ' is {}'.format('handsome'))

 also print(st + ' is {a}'.format('a = handsome'))

 or

 st = "Vytautas"
 print(f'His name is {st}') # Came in python 3.6


 **Note: float formatting follows "{value:width.precision f}"

 .format() => also work for floats

 Ex:

 value = 0.128700

 print('The result was {r:1.3f}'.format(r = value))

- List:
 Is basically a dynamic Array, can be access with [].

 In python the -1 by default is the last index of a list.

 List like strings can be access like:

 list[1:] # Index 1 to the last one.

 You can concatenate lists like list_1 + list_2 => returns one array with all the elements of both. # In Js it will return a string. 

 **Note:
 type() => returns the data type of a variable or expression.
 id(x) => returns id the memory address where x is stored.

 In python None is like undefined in JS.

 * Methods:

 .append() => Add an element to the last position on the list.
 .pop() => Remove the last element on the list.
 .sort() => It doesn't return anything, just sorts the list in place.
 .reverse() => reverse the orders of elements in the list in place(doesn't return anything)

- Dictionaries:
 Are unordered mappings for storing objects. Dictionaries use the key:value pair.

 Differences between Lists and Dictionaries:

 Dictionaries => Objects retrieve by key name, unordered and can not be sorted.

 Lists => Objects retrieve by location, ordered and can be indexed or slice.

 dictionaries can be created by {} and can be access by []. You can add a new key also with dict['new key] = 'new value'
 or change a value in a key.

 * Methods:
 .keys() => returns all the keys as a dict_keys object.
 .values() => return all the values as a dict_keys object.
 .items() => return key value pairs in tuples.

- Tuples:

 Are very similar to lists. However they have one key difference- IMMUTABILITY. Once an element is inside a tuple, it can not be REASSIGNED. It keeps the data integrity.

 Tuples use parenthesis: (1,2,3)

 * Methods:
 .count() => the times the argument is in the tuple.
 .index() => the index of the argument.

- Sets:

 Are unordered collections of UNIQUE elements(can't be repeated). Meaning there can only be one representative of the same object.

 Ex:

 myset = set()

 myset.add(1)
 # => {1}  # Is not like a dictionary because it doesn't use the key: value relationship.

 myset.add(2)
 # => {1,2}

 myset = set('Hello')
 # => {'H','e','l','l','o'} # In this case 

- Booleans:

 In python you have to type True or False with caps, it won't work otherwise.

- I/O with Basic files:

 %%writefile myfile.txt

 myfile = open('myfile.txt') # If you want to open files on another location just type the absolute path of the file

 * Methods:

 myfile.read() => returns the txt inside the file.
 .seek() => finds whatever is passed as argument.
 .readlines() => will return every line with the break on a list.
 .close() => after you finish with the file you need to close it

 with open('myfile.txt', mode = 'w') as my_new_file: # assigning to the variable
  content = my_new_file.read() 
 # with this you don't need to worry of closing a file.

 mode: w, r, a, w+, r+







 















