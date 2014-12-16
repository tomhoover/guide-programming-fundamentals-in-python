#Programming Fundamentals in Python

Approximate time ~ 1 hour

##Introduction
###What is Python?
Python is a [scripting programming language](http://en.wikipedia.org/wiki/Scripting_language) known for both its simplicity and wide breadth of applications. For this reason it is considered one of the best languages for beginners. Used for everything from Web Development to Scientific Computing, Python is referred to as a “general purpose” language by the greater programming community.

Many Python programmers (aka “Pythonistas”) love this language because it maintains a certain philosophy of best practices, described in [Tim Peter’s famous “Zen of Python”](https://www.python.org/dev/peps/pep-0020/). There is a large Python community both off and online that is welcoming and supportive of beginners, and you can find a plethora of additional materials in the resources section of this guide.

###About this Guide:
This guide will follow Thinkful’s [project-driven learning philosophy](http://blog.thinkful.com/post/100829199278/project-based-v-s-project-driven-learning), i.e. ”all concepts are taught within the context of that project and students learn as they build”. You will be creating a “Pypet” (“Python-pet”) of your choosing. As you learn new Python concepts you will be able to add new features to your Pypet. This way you will be able to put your new knowledge to use right away and actually create a project in Python.

This guide will assume no programming knowledge. You will be using a tool called Nitrous to set up your developer environment which will make it very easy to quickly get started. After this guide you will feel comfortable using Python fundamentals and have a "Pypet" to show off!

###Choose your Pypet:
Go ahead and choose a Pypet now so that we can begin! Feel free to customize your Pypet, but here are a few options. Try to keep you Pypet height limited to just one line for now as it will make the initial steps easier to follow.

####Pycat

(=^o.o^=)__

####Pymouse

<:3 )~~~~

####Pyfish

<`)))><

####Py? (you choose!)

(^‘*m*’^)

##Setup

###Nitrous.IO
The first stage of our journey will be setting up a development environment which you can work in – your Nitrous.IO box. Nitrous.io is the faster way to get your Python development environment up and running. Not only is Nitrous an amazing tool but it is also free!

####Setting up Nitrous.IO:

1. Create a [Nitrous.io](https://www.nitrous.io/) Account.
2. When it's to create your first box, choose the Python/Django option. Once that’s complete you should click the IDE button to be taken to it.
3. Now you have a powerful, cloud-based development environment that comes pre-installed with Python! Let's take a quick tour:

    - In the left-most panel, you’ll see the File Browser. Here you can navigate the files in your home folder. At this point, you will just have the "workspace" folder and a README file introducing you to Nitrous.IO. When you have more files, you can open them in Nitrous.IO’s text editor by double clicking on them in the File Broswer.
    - The middle panel is the Text Editor. This is where you can write and edit code.
    - The right panel is for chatting if you’re using Nitrous.io in collaborative mode. Close this window for now by clicking the X in the upper right hand corner so you get more screen real estate.
    - The bottom panel is your console for actually running your python file.

###Running Python for the first time!

Let’s make your first python program! Create a new file containing the following code:

```py
print 'Welcome to Pypet!'
```

You’ve just written your first print statement. Go ahead and save the file as “pypet.py”. 

Now type “python pypet.py” into your Nitrous console (in the bottom panel) and hit enter. The console will now print out “Welcome to Pypet!” This print statement is a python function for printing in the console.

If you're stuck, watch the gif below or tweet [@Thinkful](https://twitter.com/thinkful). We'd love to help!

![](http://i.imgur.com/kDyVy2I.gif)

##Creating your Pypet

The Pypet you will create is going to have certain attributes. For example we need to give it a name. Below we have set a variable called **name** equal to 'Mr Fluffy'.  In Python, variables store different types of data. 

```py
name = 'Mr Fluffy'
```

In this case, name is something called a **string** because 'Mr Fluffy' has quotations around it. A **string** is just a set of characters surrounded by quotations. Variables on the other hand do not have quotations. Let’s look at some additional data types.

```py
weight = 9.5
hungry = False
```

A **Boolean** stores a value of either True or False. A **float** is a number that can have decimals. An **integer** is a whole number. Don't use quotations for these three data types. Next, we'll include another variable that is a string containing “photo” of our pet!

```py
name = 'Mr Fluffy'
hungry = False
weight = 9.5
toys = 5
photo = '(=^o.o^=)__'
```

We need a way to tell Python that all of these variables represent one cat. One way to do this is to use a Python dictionary. Dictionaries are a way of storing multiple variables that contain different values.

```py
cat = {
  'name': 'Mr Fluffy',
  'hungry': True,
  'weight': 9.5,
  'number_of_toys': 5,
  'photo': '(=^o.o^=)__',
}

print cat
```

Here we’ve created an empty dictionary called cat = {}. Each line contains a different cat attribute. The attribute described is called a "key" (ex. name, weight, number_of_toys) while the value of each attribute is called...you guessed it - value! 

Next, we've added a print statement to view our first pypet in the console. Try it yourself! Use different "key:value" pairs to customize your own pypet in the text editor (the right panel).

GIF HERE?

##Feeding your Pypet - Functions and If Statements

Now we are going learn how to “feed” your pypet using a Python function. A [function](http://www.tutorialspoint.com/python/python_functions.htm) is a block of organized, reusable code that is used to perform a single, related action. First, we must define our function. This particular feed() function changes our pypet’s “hungry” attribute to False to show that it is no longer hungry.

```py
def feed(pet):
		pet['hungry'] = False
```

Now that you have defined your function you can use it by adding **feed(cat)** to your code.

```py
def feed(pet):
		pet['hungry'] = False

feed(cat)
```

By calling feed(cat) we are passing the variable cat into the function in place of ‘pet’.

We should also increase the Pypet’s weight a bit since it has eaten. Floats and integers can be increased by using the following notation.

```py
def feed(cat):
		cat['hungry'] = False
		cat['weight'] = cat['weight'] + 1
```

Try setting your original pypet’s hungry variable to True and then call the function by writing feed(cat) at the bottom like so:

```py
print 'Welome to Pypet!'

cat = {
  'name': 'Mr Fluffy',
  'hungry': True,
  'weight': 9.5,
  'number_of_toys': 5,
  'photo': '(=^o.o^=)__',
}

print cat

def feed(pet):
		pet['hungry'] = False
		pet['weight'] += 1

feed(cat)

print cat
```

When the cat is printed out the second time his weight attribute will have increased. But what if our pypet is not hungry? We need to take into account whether or not the hungry variable is set to True or False.

In order to know whether our Pypet is hungry, we are going to use an if statement. If the Pypet is hungry the program will set his hungry variable to False and increase his weight. If the Pypet is not hungry then it will print ‘The Pypet is not hungry! in the console. Try feeding the cat twice, to make sure that the if statement worked

```py
print 'Welome to Pypet!'

cat = {
  'name': 'Mr Fluffy',
  'hungry': True,
  'weight': 9.5,
  'number_of_toys': 5,
  'photo': '(=^o.o^=)__',
}

def feed(cat):
	if cat['hungry']:
		cat['hungry'] = False
		cat['weight']+=1
	else:
		print 'The Pypet is not hungry!'

print cat
feed(cat)
feed(cat)
print cat
```

YOU CAN ADD THE CONCATENATE BIT IF YOU HAVE ROOM.


##Friends for your Pypet! - For Loops and Lists

FUN HERE!!Let’s create another Pypet!

```py
mouse = {
  'name': 'Mouse',
  'hungry': False,
  'weight': 1.5,
  'number_of_toys': 6,
  'photo': '<:3 )~~~~',
}
```

Now that we have more than one Pypet we can store them in a Python list. A [list](http://www.tutorialspoint.com/python/python_lists.htm) is another data type; lists stores variables in order:

```py
pets = [cat, mouse]
```

What if we want to feed all the pets in our list? If we want to run a function on each variable in a list we can use something in Python called a for loop. The [for loop](http://www.tutorialspoint.com/python/python_for_loop.htm) in Python has the ability to iterate over the items of any sequence, such as a list or a string.

```py
for pet in pets:
	feed(pet)
print pet
```

Call to Action - tweet a picture of your pypets [@Thinkful](https://twitter.com/thinkful) so we can share your creation with the world

BONUS/ADVANCED FEATURES SECTION: Perhaps you want to keep track of health points or create a play() function?

##Conclusion & Resources

This guide is just the beginning of what you can do with Python. If you enjoyed the work you’ve done here, go through any of the additional resources below. If you are stuck feel free to tweet [@Thinkful](https://twitter.com/thinkful) and we would love to help you. Feel free to customize any or all of your project and try new things. We have placed a final version of our Pypet [on github](https://github.com/TatianaTylosky/pypet/blob/master/pypet.py) if you would like to take a look at the code! 

http://learnpythonthehardway.org/

NEED MORE RESOURCES



