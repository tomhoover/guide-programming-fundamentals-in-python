#Programming Fundamentals in Python

Approximate time ~ 1 hour

##Introduction

###About this Guide:

This guide was created for complete beginners and will teach you programming fundamentals in Python. Following Thinkful’s [project-driven learning philosophy](http://blog.thinkful.com/post/100829199278/project-based-v-s-project-driven-learning) you will learn by actually building your own project. We also use Gifs throughout this guide to make everything as clear as possible.

As you complete this guide you'll learn Python fundamentals by creating a virtual pet we'll call "Pypet" (a "Python-pet"). Think of your Pypet as a modern-age tamagochi or Pokemon! With each new Python programming concepts you will add new features to your Pypet putting your knowledge to the test.

There are no software or computer requirements for this guide except that you need access to a web broswer (which you obviously already have at this point). You will learn how to use a free tool called [Nitrous](https://www.nitrous.io/) to set up your developer environment which takes away the typical pain of setting up a coding environment. It is also cloud based so you can log in from any computer to view your code.

###What is Python?

Python is a [scripting programming language](http://en.wikipedia.org/wiki/Scripting_language) known for both its simplicity and wide breadth of applications. For this reason it is considered one of the best languages for beginners. Used for everything from Web Development to Scientific Computing, Python is referred to as a “general purpose” language by the greater programming community.

Many Python programmers (aka “Pythonistas”) love this language because it maintains a certain philosophy of best practices, described in [Tim Peter’s famous “Zen of Python”](https://www.python.org/dev/peps/pep-0020/). There is a large Python community both off and online that is welcoming and supportive of beginners, and you can find a plethora of additional materials in the [resources]() section of this guide.

##Setup

To get started, we'll need a development environment, aka a place to write and execute code. For this we'll use [Nitrous.io](https://www.nitrous.io/), a fast and free way to get you up and running. Nitrous is a cloud-based developer environment that works really well for programming in python. We are using it because it won't matter whether you use mac or windows or any other operating system in order to run and test your code.

*******rewrite this to make it really clear
*******add gif for this

1. Go to [Nitrous.io](https://www.nitrous.io/) and create an account. NOTE:You will have to check your email and activate your account before you can sign in.
2. Once you have signed in and confirmed your email click the "open dashboard" button on their [homepage](https://www.nitrous.io/).
3. You should be prompted to create your first Nitrous "box" aka developer environment. Choose "Python/Django". You can rename your box anything you like or just leave it as is. Don't worry about the optional section that says "Download a Github repo". See image below as an example.
![](http://i.imgur.com/gBTqt8X.png)

4. Click "Create Box" and then click "Next" until you can see your box. Click on your box and then the button that says IDE. Now you have a powerful, cloud-based development environment that comes pre-installed with Python!

5. Let's take a quick tour:
![](http://i.imgur.com/6bXzy6A.png)
    - In the left-most panel, you’ll see the File Browser. Here you can navigate the files in your home folder. At this point, you will just have the "workspace" folder and a README file introducing you to Nitrous.IO. When you have more files, you can open them in Nitrous.IO’s text editor by double clicking on them in the File Broswer.
    - The middle panel is the Text Editor. This is where you can write and edit code.
    - The right panel is for chatting if you’re using Nitrous.io in collaborative mode. Close this window for now by clicking the X in the upper right hand corner so you get more screen real estate.
    - The bottom panel is your console for actually running your python file.

##Running Python for the first time

Here is a Gif demonstrating how to run your first python program. Feel free to either skip down and read the steps in the text below or take a look at the Gif first.

![](http://i.imgur.com/kDyVy2I.gif)

-------------

1. Create a new file containing the following code:

```py
print 'Welcome to Pypet!'
```
You’ve just written your first print statement. 

2. Go ahead and save the file as “pypet.py”. 

3. Now type “python pypet.py” into your Nitrous console (in the bottom panel) and hit enter. 

The console will output “Welcome to Pypet!”. This print statement is a python function which prints things in the console — it's very handy for learning Python and debugging your code.

-------------

If you're stuck, take another look at the gif above or tweet [@Thinkful](https://twitter.com/thinkful). We'd love to help!

##Creating your Pypet

The Pypet you will create is going to have certain attributes. For example we need to give it a name.

1. Create a variable called `name` equal to `'Mr Fluffy'`.

```py
name = 'Mr Fluffy'
```
In Python, variables store different types of data. In this case, name is something called a **string** because 'Mr Fluffy' has quotations around it. A **string** is just a set of characters surrounded by quotations. Variables on the other hand do not have quotations. Let’s look at some additional data types.

2. Create three additional variables to track hunger, weight and toys.

```py
name = 'Mr Fluffy'
hungry = False
weight = 9.5
toys = 5
```

The `hungry` variable is a a **Boolean**. Booleans stores a value of either `True` or `False`. The `weight` variable is a **float**. Floats are a numbers that can have decimals. Last the `toys` variable is an **integer** which must be a whole number. NOTE: Don't use quotations for these three data types.

3. Choose your Pypet's "photo". We've included a few options you can use below, but feel free to customize it. 
NOTE:Keep you Pypet height to just one line as it will make the initial steps easier to follow.

####Pycat

(=^o.o^=)__

####Pymouse

<:3 )~~~~

####Pyfish

<`)))><

####Py? (you choose!)

(^‘*m*’^)

6. Next include another variable that is a string containing this “photo” of our pet.

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

__Note for Tati:__ Am I supposed to follow along here or are you just explaining stuff? I'm not sure what I'm supposed to do from the last note up until here. My vote would be to hand-hold the reader through each one of these steps.

__Note for Tati:__ Why do variables get an equal sign '=' while object keys get a colon ":"? We should explain this.

Here we’ve created an empty dictionary called cat = {}. Each line contains a different cat attribute. The attribute described is called a "key" (ex. name, weight, number_of_toys) while the value of each attribute is called...you guessed it - value!

Next, we've added a print statement to view our first pypet in the console. Try using different "key:value" pairs to customize your pypet in the text editor.

![](http://i.imgur.com/bsj0LGE.gif)

##Feeding your Pypet - Functions and If Statements

Let's “feed” our pypet using a Python function. A [function](http://www.tutorialspoint.com/python/python_functions.htm) is a block of organized, reusable code that is used to perform a single action. First, we must define our function — `feed` — which changes our pypet’s “hungry” attribute to False to show that it is no longer hungry.

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

__Note for Tati:__ We haven't introduced how to access values inside an object, there's a gap here. Also, we haven't talked about indentation and how that works in Python. Lastly, we haven't mentioned that the quotes (e.g. 'feed()') call a function. It might be useful to show a "hungry cat" before feeding it, feed it, and then show that it's no longer hungry.

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
  'name': 'Mr Fluffy',
  'hungry': True,
  'weight': 9.5,
  'number_of_toys': 5,
  'photo': '(=^o.o^=)__',
}

def feed(pet):
	if pet['hungry']:
		pet['hungry'] = False
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
  'hungry': False,
  'weight': 1.5,
  'number_of_toys': 6,
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
