#Programming Fundamentals in Python

Approximate time ~ 1 hour

##Introduction

###About this Guide:

Learning promise*****
__Note for Tati:__ The intro doesn't tell me what I'm going to learn (e.g. data structures) and it doesn't tell me who this is right for (e.g. total beginners). This needs some TLC. Also, is "Pypet" a python thing or a this guide thing? I'm confused. Adding the tamagochi referrence might help.
> You will learn Python fundamentals by creating a virtual pet we'll call "Pypet" (a "Python-pet"). Think of your Pypet as a modern-age tamagochi.

This guide will follow Thinkful’s [project-driven learning philosophy](http://blog.thinkful.com/post/100829199278/project-based-v-s-project-driven-learning), i.e. ”all concepts are taught within the context of that project and students learn as they build”. You will be creating a “Pypet” (“Python-pet”) of your choosing. As you learn new Python concepts you will add new features to your Pypet, allowing to put your knowledge to the test.

We use Gifs throughout this guide to make everything as clear as possible.

This guide assumes no programming knowledge. You will be using a tool called [Nitrous](https://www.nitrous.io/) to set up your developer environment which makes it easy to get started.

###What is Python?

Python is a [scripting programming language](http://en.wikipedia.org/wiki/Scripting_language) known for both its simplicity and wide breadth of applications. For this reason it is considered one of the best languages for beginners. Used for everything from Web Development to Scientific Computing, Python is referred to as a “general purpose” language by the greater programming community.

Many Python programmers (aka “Pythonistas”) love this language because it maintains a certain philosophy of best practices, described in [Tim Peter’s famous “Zen of Python”](https://www.python.org/dev/peps/pep-0020/). There is a large Python community both off and online that is welcoming and supportive of beginners, and you can find a plethora of additional materials in the resources section of this guide.

###Choose your Pypet:
To get started you'll need to choose a Pypet. We've included a few options you can use, but feel free to customize it. Keep you Pypet height to just one line as it will make the initial steps easier to follow.

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
To get started, we'll need a development environment. For this we'll use [Nitrous.io](https://www.nitrous.io/), a fast and free way to get a Python development environment up and running. Nitrous is a X. We are using it because Y.

####Setting up Nitrous.IO:

*******rewrite this to make it really clear
*******add gif for this

1. Create a [Nitrous.io](https://www.nitrous.io/) account.
2. Once you've confirmed your email, create a Python/Django box. Once your box is ready, click the IDE button.
3. Now you have a powerful, cloud-based development environment that comes pre-installed with Python. Let's take a quick tour:

    - In the left-most panel, you’ll see the File Browser. Here you can navigate the files in your home folder. At this point, you will just have the "workspace" folder and a README file introducing you to Nitrous.IO. When you have more files, you can open them in Nitrous.IO’s text editor by double clicking on them in the File Broswer.
    - The middle panel is the Text Editor. This is where you can write and edit code.
    - The right panel is for chatting if you’re using Nitrous.io in collaborative mode. Close this window for now by clicking the X in the upper right hand corner so you get more screen real estate.
    - The bottom panel is your console for actually running your python file.

make sure you covered all of this******
__Note for Tati:__ This needs screenshots. Make sure you use the same language as the app: they don't use the "IDE" language, they say "Okay, take me to my box". What is "cloud-based development environment"? I'm a n00b try to avoid technical terms unless you explain them. Why are we using Nitrous? Explaining that we're doing this to simplify the follow-along for everyone is key... if not I'm thinking: "But hey, I have Python on my mac. Could I use Python on my mac? Do I NEED to use nitrous?". Do I need to have a Nitrous.io quick tour now? Can I not learn to use this thing as we go? If I need this now, is text the best way to do it (v.s. video)?

###Running Python for the first time

Here is a Gif demonstrating how to run your first python program. Feel free to either skip down and read the steps in the text below or take a look at the Gif first.

![](http://i.imgur.com/kDyVy2I.gif)

-------------

1. To make our first python program, let's create a new file containing the following code:

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

The Pypet you will create is going to have certain attributes. For example we need to give it a name. Let's create a variable called **name** equal to 'Mr Fluffy'.  In Python, variables store different types of data. 

```py
name = 'Mr Fluffy'
```

In this case, name is something called a **string** because 'Mr Fluffy' has quotations around it. A **string** is just a set of characters surrounded by quotations. Variables on the other hand do not have quotations. Let’s look at some additional data types.

```py
hungry = False
weight = 9.5
```

A **Boolean** stores a value of either True or False. A **float** is a number that can have decimals. An **integer** is a whole number. Don't use quotations for these three data types. Next, we'll include another variable that is a string containing “photo” of our pet.

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

Now that we have more than one Pypet we can store them in a Python list. A [list](http://www.tutorialspoint.com/python/python_lists.htm) is another data type; lists stores variables in order:

```py
pets = [cat, mouse]
```

__Note for Tati:__ I would mention that in other programming languages lists are often referred to as "array".

What if we want to feed all the pets in our list? If we want to run a function on each variable in a list we can use something in Python called a loop. The [for loop](http://www.tutorialspoint.com/python/python_for_loop.htm) in Python has the ability to iterate over the items of any sequence, such as a list or a string.

```py
for pet in pets:
	feed(pet)
print pet
```

__Note for Tati:__ Show me how to use this on a string, since we mention it.

Call to Action - tweet a picture of your pypets [@Thinkful](https://twitter.com/thinkful) so we can share your creation with the world.

BONUS/ADVANCED FEATURES SECTION: Perhaps you want to keep track of health points or create a play() function?

__Note for Tati:__ What is this bonus about? Feels like something is missing.

##Conclusion & Resources

This guide is just the beginning of what you can do with Python. If you enjoyed the work you’ve done here, go through any of the additional resources below. If you are stuck feel free to tweet [@Thinkful](https://twitter.com/thinkful) — we would love to help you. Feel free to customize any or all of your project and try new things. We have placed a final version of our Pypet [on github](https://github.com/TatianaTylosky/pypet/blob/master/pypet.py) if you would like to take a look at the code.

__Note for Tati:__ This should live under a Thinkful repo (not a TatianaTylosky repo).

Free Resources:
- [Learnpythonthehardway.org](http://learnpythonthehardway.org/)
- [Learn Python on Codecademy](http://www.codecademy.com/en/tracks/python)
- [Think Python](http://www.greenteapress.com/thinkpython/)

Free tools:
- [IPython Notebook](http://ipython.org/notebook.html)
