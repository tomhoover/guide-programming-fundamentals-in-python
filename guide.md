#Programming Fundamentals in Python

Approximate time ~ 1 hour

##Introduction

###About this Guide:

This guide was created for complete beginners and will teach you programming fundamentals in Python. Following our [project-driven learning philosophy](http://blog.thinkful.com/post/100829199278/project-based-v-s-project-driven-learning) you will learn as you build your own project. There will be GIFs and screenshots throughout this guide to make everything as clear as possible.

As you complete this guide you'll be creating a virtual pet we'll call "Pypet" (a "Python-pet"). Think of your Pypet as a modern-age tamagochi or Pokemon! With each new Python programming concepts you learn you will add new features to your Pypet.

There are no software or computer requirements for this guide except that you need access to a web broswer (which you obviously already have at this point). You will learn how to use a free tool called [Nitrous](https://www.nitrous.io/) to set up your developer environment which takes away the typical pain of setting up a coding environment. It is also cloud based so you can log in from any computer to view your code.

###What is Python?

Python is a [scripting programming language](http://en.wikipedia.org/wiki/Scripting_language) known for both its simplicity and wide breadth of applications. For this reason it is considered one of the best languages for beginners. Used for everything from Web Development to Scientific Computing, Python is referred to as a “general purpose” language by the greater programming community.

Many Python programmers (aka “Pythonistas”) love this language because it maintains a certain philosophy of best practices, described in [Tim Peter’s famous “Zen of Python”](https://www.python.org/dev/peps/pep-0020/). There is a large Python community both off and online that is welcoming and supportive of beginners, and you can find a plethora of additional materials in the [resources]() section of this guide.

##Setup

To get started we'll need a development environment, aka a place to write and execute code. For this we'll use [Nitrous.io](https://www.nitrous.io/), a fast and free way to get you up and running. Nitrous is a cloud-based developer environment that works really well for programming in python. Since Nitrous.io is a web application it won't matter whether you have a mac or windows or even linux computer to run and test your code. Follow the instructions below to set up your Nitrous.io Development Environment.

1. Go to [Nitrous.io](https://www.nitrous.io/) and create an account. NOTE: You will have to check your email and activate your account before you can sign in.
2. Once you have signed in and confirmed your email click the "open dashboard" button on their [homepage](https://www.nitrous.io/). You should be prompted to create your first Nitrous "box" aka developer environment.
3. First choose "Python/Django" as your template. Next you can rename your box anything you like or just leave it as is. Finally don't worry about the optional section that says "Download a Github repo". See image below as an example:

	![](http://i.imgur.com/gBTqt8X.png)

4. Click "Create Box" and then click "Next" until you can the box name you previously chose. Click on your box and then the button that says [IDE](https://en.wikipedia.org/wiki/Integrated_development_environment). Now you have a powerful, cloud-based development environment that comes pre-installed with Python!

5. Let's take a quick tour:
![](http://i.imgur.com/6bXzy6A.png)
    - In the **left panel**, you’ll see the File Browser. Here you can navigate the files in your home folder. At this point, you will just have the "workspace" folder and a README file introducing you to Nitrous.IO. When you have more files, you can open them in Nitrous.IO’s text editor by double clicking on them in the File Broswer.
    - The **middle panel** is the Text Editor. This is where you can write and edit code.
    - The **right panel** is for chatting if you’re using Nitrous.io in collaborative mode. Close this window for now by clicking the X in the upper right hand corner so you get more screen real estate.
    - The **bottom panel** is your console for actually running your python file.

##Running Python for the first time

Here is a Gif demonstrating how to run your first python program. Feel free to either skip down and read the steps in the text below or take a look at the Gif first.

![](http://i.imgur.com/kDyVy2I.gif)

1. Create a new file containing the following code in the text editor (middle panel):

	```py
	print 'Welcome to Pypet!'
	```

2. Go ahead and save the file as “pypet.py”. 

3. Now type `python pypet.py` into your Nitrous console (in the bottom panel) and hit enter. By doing this you are telling your console to open the file `pypet.py` and execute it using the program called `python`. The console will output “Welcome to Pypet!”.

![](http://i.imgur.com/0YqbGNh.png)

You’ve just written your first print statement. The print statement is a python function which prints things in the console — it's very handy for learning Python and debugging your code.

If you're stuck, take another look at the gif above or tweet [@Thinkful](https://twitter.com/thinkful). We'd love to help!

##Creating your Pypet

###Variables

Variables are a way of storing information in Python. Below we'll create different variables for our pypet such as name, weight, etc.

1. Create a variable called `name` equal to `'Fluffy'`.
	
	```py
	print 'Welcome to Pypet!'
	
	name = 'Fluffy'
	```
	Variables can store different types of data. In this case, `name` is something called a **string** because `'Fluffy'` 		has quotations around it. A **string** is just a set of characters surrounded by quotations (for example 'Bob' or 'New 	York'). *NOTE: strings can use 		either single or double quotes.* **Integers** on the other hand	do not have 			quotations. Let’s look at some additional 	data types.
	
2. Create three additional variables to track age, weight and hunger.

	```py
	print 'Welcome to Pypet!'
	
	name = 'Fluffy'
	age = 5
	weight = 9.5
	hunger = False
	```
	
	The `age` variable is an **integer** and therefore must be a whole number. The `weight` variable is a **float**. Floats 	are a numbers that can have values after the decimal point.  The `hunger` variable is a a **Boolean**. Booleans stores 	a value of either `True` or `False`. *NOTE: Don't use quotations for these three data types.*

3. Choose your Pypet's "photo". We've included a few options you can use below, but feel free to customize it. 
*NOTE: Keep your Pypet's "photo" to just one line as it will make the initial steps easier to follow.*

	--------------------------
	####Pycat
	
	(=^o.o^=)__
	
	####Pymouse
	
	<:3 )~~~~
	
	####Pyfish
	
	<`)))><
	
	####Py? You choose!
	
	(^‘0M0’^)
	
	--------------------------

4. Next include another variable that is a **string** containing this “photo” of our pet.

	```py
	print 'Welcome to Pypet!'
	
	name = 'Fluffy'
	age = 5
	weight = 9.5
	hunger = False
	photo = '(=^o.o^=)__'
	```

5. Add some print statements to your code so you can see your Pypet in the console.

	```py
	print 'Welcome to Pypet!'
	
	name = 'Fluffy'
	age = 5
	weight = 9.5
	hunger = False
	photo = '(=^o.o^=)__'
	
	print 'Hello ' + name + '!'
	print photo
	```
	Don't forget to run `python pypet.py` in the console (bottom window). Your console should look like:
	
	![](http://i.imgur.com/teThhJk.png)
	
###Dictionaries

We need a way to tell Python that all of these variables represent one cat (or dog, fish, creature etc). One way to do this is to use a Python **dictionary**. Dictionaries are a way of storing multiple variables that contain different values. Here is another Gif that you can refer back to as you follow along with the instructions below.

![](http://i.imgur.com/bsj0LGE.gif)

1. Place your variables in a dictionary. Try using different "key:value" pairs to customize your pypet in the text editor.

	```py
	print 'Welcome to Pypet!'
	
	cat = {
	  'name': 'Fluffy',
	  'hunger': True,
	  'weight': 9.5,
	  'age': 5,
	  'photo': '(=^o.o^=)__',
	}

	```
	Here we’ve created a dictionary called `cat`. Each line contains a different cat attribute. Attributes have both a 		"key" (ex. name, weight, age) as well as a value (ex. 'Fluffy', Tue, 9.6 etc). Unlike assigning variables which use an 	equals sign, dictionary attributes use a colon.

2. Add a print statement to view your pypet in the console. Don't forget to run your file in the console by typing "python pypet.py" and pressing enter

	```py
	cat = {
	  'name': 'Fluffy',
	  'hunger': True,
	  'weight': 9.5,
	  'age': 5,
	  'photo': '(=^o.o^=)__',
	}

	print cat
	```

NOTE TO SELF: DO YOU WANT TO SHOW THEM HOW TO ACCESS ATTRIBUTES

Make sure to take another look at the gif above if you get stuck.

##Feeding your Pypet - Functions and If Statements

Let's “feed” our pypet using a Python function. A [function](http://www.tutorialspoint.com/python/python_functions.htm) is a block of organized, reusable code that is used to perform a single action. First, we must define our function — `feed` — which changes our pypet’s “hungry” attribute to False to show that it is no longer hungry.

```py
def feed(pet):
		pet['hunger'] = False
```

Now that you have defined your function you can use it by adding **feed(cat)** to your code.

```py
def feed(pet):
		pet['hunger'] = False

feed(cat)
```

By calling feed(cat) we are passing the variable cat into the function in place of ‘pet’.

__Note for Tati:__ We haven't introduced how to access values inside an object, there's a gap here. Also, we haven't talked about indentation and how that works in Python. Lastly, we haven't mentioned that the quotes (e.g. 'feed()') call a function. It might be useful to show a "hungry cat" before feeding it, feed it, and then show that it's no longer hungry.

We should also increase the Pypet’s weight a bit since it has eaten. Floats and integers can be increased by using the following notation.

```py
def feed(cat):
		cat['hunger'] = False
		cat['weight'] = cat['weight'] + 1
```

Try setting your original pypet’s hungry variable to True and then call the function by writing feed(cat) at the bottom like so:

```py
print 'Welome to Pypet!'

cat = {
  'name': 'Fluffy',
  'hungry': True,
  'weight': 9.5,
  'age': 5,
  'photo': '(=^o.o^=)__',
}

print cat

def feed(pet):
		pet['hunger'] = False
		cat['weight'] = cat['weight'] + 1

feed(cat)

print cat
```

__Note for Tati:__ What's the expected results here? Show it. What might go wrong as I do this? Help me debug popular errors.

When the cat is printed out the second time his weight attribute will have increased. But what if our pypet is not hungry? We need to take into account whether or not the hungry variable is set to True or False.

In order to know whether our Pypet is hungry, we are going to use an if statement. If the Pypet is hungry the program will set his hungry variable to False and increase his weight. If the Pypet is not hungry then it will print ‘The Pypet is not hungry' in the console. Try feeding the cat twice, to make sure that the if statement worked

```py
print 'Welome to Pypet!'

cat = {
  'name': 'Fluffy',
  'hunger': True,
  'weight': 9.5,
  'age': 5,
  'photo': '(=^o.o^=)__',
}

def feed(pet):
	if pet['hunger']:
		pet['hunger'] = False
		pet['weight'] = pet['weight'] + 1
	else:
		print 'The Pypet is not hungry!'

print cat
feed(cat)
feed(cat)
print cat
```

__Note for Tati:__ what is this gif showing me? All I see is you writing code... not sure what the gif is showing me since it prints that the pypet is not hungry twice (your fish hungry is set to false in the example).

![](http://i.imgur.com/Axp2Smt.gif)

##Friends for your Pypet - For Loops and Lists

Let’s create another Pypet:

```py
mouse = {
  'name': 'Mouse',
  'hunger': False,
  'weight': 1.5,
  'age': 6,
  'photo': '<:3 )~~~~',
}
```

Now that we have more than one Pypet we can store them in a Python list. A [list](http://www.tutorialspoint.com/python/python_lists.htm) is another data type; lists stores variables in order. If python isn't the first programming language you are learning, you may have heard of this same concept in other programming languages as an [array](http://techterms.com/definition/array).

```py
pets = [cat, mouse]
```

What if we want to feed all the pets in our list? If we want to run a function on each variable in a list we can use something in Python called a loop. The [for loop](http://www.tutorialspoint.com/python/python_for_loop.htm) in Python has the ability to iterate over the items of any sequence, such as a list.

```py
for pet in pets:
	feed(pet)
print pet
```

Tweet a screenshot of your pypets [@Thinkful](https://twitter.com/thinkful) so we can share your creation with the world!

BONUS: 
Once you have completed the steps above you should feel free to add additional features that you design yourself! Here are some ideas to get you started:

- keep track of a health points variable
- create a `play()` function
- create a boolean variable for sleep

##Conclusion & Resources

Congrats for reaching the end of this guide! For your convenience we've placed a final version of our Pypet [on github](https://github.com/Thinkful/pypet/blob/master/pypet.py) if you would like to take a look at the code. If you are stuck tweet [@Thinkful](https://twitter.com/thinkful) and we'd love to help. Feel free to customize any or all of your project and try new things.

This guide is just the beginning of what you can do with Python. If you enjoyed the work you’ve done here, go through any of the additional resources below. 

Free Resources:

- [The Hitchhiker's Guide to Python!](http://docs.python-guide.org/en/latest/)
- [Coursera - Interactive Python](https://www.coursera.org/course/interactivepython)
- [Learn Python the Hard Way](http://learnpythonthehardway.org/)
- [Invent With Python](http://inventwithpython.com/)
- [Green Tea Press](http://greenteapress.com/)
- [Codecademy](http://www.codecademy.com/#!/exercises/0)
- [Dive Into Python](http://www.diveintopython.net/)
- [Real Python](http://www.realpython.com/)
