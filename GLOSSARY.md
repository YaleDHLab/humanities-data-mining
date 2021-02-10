## Glossary

We can use this glossary to keep track of technical words introduced in the course of the class. If there are words you'd like to add, please let us know!

### Algorithms

Algorithms are a set of instructions that tell the computer what to do and how to do it.

### Argument

Arguments are the pieces of data we pass into a function. For example, consider the following code snippet:

```python
greeting = 'Hello world!'

print(greeting)
```

In that code snippet, `print` is the function we are calling, and the variable `greeting` is the argument to that function. In other words, the variable `greeting` is the data we are providing to the `print` function.

Once the `print` function receives that data, it will display the value assigned to the input data. In our case above, the value of the variable `greeting` is `'Hello world!'`, so that string will be displayed by the function.

### Call

The verb "call" is often used to signify that one is evoking a function. For example, consider the code block below:

```python
my_name = 'Jonathan Swift'

corrected = my_name.replace('Jonathan', 'Taylor')
```

We would say the code snippet above "calls" the replace method on `my_name`.

### Corpus

Corpus signifies a collection of texts. The word is often used in text mining to refer to all of the texts underlying a project.

### Declare

The verb "declare" is often used to indicate that one is defining a variable. For example, consider the following code block:

```python
lucky_number = 24
```

This line defines a new variable (`lucky_number`) and sets the value of that variable to 24. In other words, this line "declares" the variable `lucky_number`. In noun form, the line above is an example of "variable declaration".

Note that the verb "declare" is generally only used to refer to the act of defining a variable for the first time. If you were to change the value assigned to an extant variable, the preferable verb would be "reassign", as in "I delcared the variable on line one and then reassigned it on line two".

### Function

Functions are pieces of programs that transform data. We saw some examples of functions as early as week one:

```python
print('Howdy neighbor!')
```

In the example above, `print()` is a function. Functions end with rounded parentheses, so they are generally pretty easy to identify!

### Index Position

The "index position" of an item is the item's position within some larger object. Consider for example the following list:

```python
stooges = ['Larry', 'Curly', 'Moe']
```

In this list, 'Larry' is at index position 0 because he is the first in the list and Python starts counting at 0. Next is Curly, who is at index position 1. Finally we have Moe, who is at index position 2. In short, index position just indicates the location of some object in some larger object.

### Introspection

Introspection refers to looking inside a variable to see what's inside. In week one, we saw that we can peer inside of an object to see the methods and attributes available on that object using the `dir()` function:

```python
opening_song = 'BWV 988'

dir(opening_song)
```

In the snippet above, the `dir()` function lets us look inside the `opening_song` variable to see the methods and attributes defined inside.

### Instantiate

The verb "instantiate" is synonymous with "declare". To instantiate a variable just means to define the variable for the first time.

### List

Lists are a fundamental datatype. They store sequences of objects. Let's see an example:

```python
numbers = [1, 2, 3]
```

The list above contains three objects. In general, lists are useful for representing multiple pieces of data inside a single variable.

### Loop

Loops let us interact with each object in an iterable. Let's see an exmaple:

```python
words = ['I', 'think', 'therefore', 'I', 'am']

for word in words:

  print(word)
```

The example above will pass each word in `words` to the indented lines underneath the for loop. In the example above, we simply print each word. In other examples, we might run more complicated operations on each item in the sequence provided to the loop.

### Metadata

Metadata is often described as "data about data." It might include, for example, information about an author or place of publication.

### Method

Methods are functions that are defined on objects. As an example, we saw in week one that strings have various methods defined within them:

```python
my_film = 'Monty Python'

dir(film)
```

The output of that `dir()` function will identify the various methods that are defined on the `my_film` variable. In the output, for example, one will find the method `upper`. This means that the string `my_film` has a method upper that we can call:

```python
my_film = 'Monty Python'

uppercased = my_film.upper()

print(uppercased)
```

If you run that code block, you should see that the value assigned to the `uppercased` variable is 'MONTY PYTHON', i.e. an uppercase version of `my_film`! As you can see in the output of the `dir(my_film)` command, `upper()` is only one of many methods we can call on strings. If you're feeling experimental, try some others and see if you can tell what they do!

### Module

Python modules are bits of code that we import into our programs. In week one, we experimented with the `collections` module in order to count words in some sample documents:

```python
import collections

word_counter = collections.Counter()
```

The example above "imports" (or makes available to our program) the `collections` module, then instantiates a new `collections.Counter()` object named `word_counter`.

In general, we will use modules to help us run data processing and visualization tasks. We'll see plenty of examples of modules throughout the semester, and we will interact with those modules by using the `import` statement to load the modules into our programs.

### Object

The term "object" is one of the more abstract concepts we will encounter this semester. In Python, "everything is an object". This means that we can use the word "object" to refer to strings, lists, functions, as are plenty of other constructs we will encounter over the course of the semester.

### Optical Character Recognition (OCR)

OCR refers to the process of converting an image of a text into searchable text. The process can be error prone, depending on the quality of the image and typeface. It also works best with printed rather than handwritten materials. For OCR software, we recommend trying [Abbyy FineReader](https://pdf.abbyy.com/).

### Parameter

The word "parameter" is used in the same way the word "argument" is used--both refer to the piece(s) of data that we pass into a function.

### String

Strings are a fundamental datatype in Python. Strings hold text data, and are recognizable by the fact that they are surrounded by quote marks:

```python
greeting_a = 'Hello!'

greeting_b = "Hello!"

greeting_c = '''Hello!'''
```

The three greetings above are all strings, and those strings are equivalent in value--the quotation marks you choose to use have no impact on the value of the string you define.

### Tokenization

Tokenization is the process of dividing a text (a sequence of strings) into meaningful units, such as words, phrases, chapters, etc. The resulting "tokens" are then used as input for data mining.

### Variable

Variables are names we make up to store some data. Let's see an example:

```python
author = 'Lewis Carroll'
```

In the line above, `author` is our variable, and `'Lewis Carroll'` is the value assigned to that variable.
