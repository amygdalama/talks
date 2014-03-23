Replacing `import` with `accio`: Compiling Pythons with Custom Grammar for the sake of a joke!

##Abstract

In Python, overwriting builtin functions is fairly easy. You can even do it in the interpreter! But can you overwrite a statement, like import, just as easily? Let's go on an adventure, discovering how the import statement works, and how Python statements are defined in the CPython source code. We'll face some consequences of bootstrapping, and, to get our custom Harry Potter-themed Grammar to work, we'll have to compile a Python to compile a Python.

##Timeline

* Builtins: What's in the `__builtin__` module and can we do mischievous things like shadow or delete builtins?
* Import: Can we shadow/delete the import statement? How does the import statement work? Is it a builtin?
* Grammar: Where is the import statement defined? We'll look at CPython's Grammar file to figure out what it means to be an import statement, and we'll try editing the Grammar file to create an accio statement instead.
* Bootstrapping: When we compile our new Python (with accio instead of import), we'll get lots of errors! Why? It turns out about half of CPython is written in Python, so compiling Python requires Python on your computer! *Mind explodes!* We'll come face-to-face with the concept of bootstrapping, and have to compile a Python to compile another Python.

##Intended Audience

Beginner? The audience will get the most out of the talk if they're familiar with basic Python syntax, like 

    :::python
    >>> import random
    >>> random.random()
    >>> dir(random)

This talk is in part intended to demystify CPython source code so that even beginners feel comfortable cloning it and fiddling around.

##Additional Links

Here are some work-in-progress slides for the talk: http://www.slideshare.net/AmyHanlon/slides-32517750

Here's the blog post I wrote that was the inspiration for this talk: http://mathamy.com/import-accio-bootstrapping-python-grammar.html

Allison Kaptur also wrote a couple related blog posts:
* http://akaptur.github.io/blog/2014/03/16/pycon-prep-import-is-a-keyword/
* http://akaptur.github.io/blog/2014/03/16/reading-ebnf/

###Bio

I'm in the W'14 batch at Hacker School, where I've worked on projects like creating sounds from spectrograms (huge failure) and replacing Python builtins and keywords with Harry Potter spells (huge success).

My background is in Theoretical Math. After college I optimized paid search ads for Adam & Eve, so I basically used to sell dildos on the internet (though my employer was Adlucent, an agency in Austin, TX). I then used machine learning via scikit-learn to automate tasks like classification of search queries into product categories.

I will nerd out with you about sex toys, programming, science fiction, feminism, comics, Dune (I <3 Dune. Dune, Dune, Dune.), math, board games, etc. I also think it's fabulous to drink champagne in bed.

###G-Rated Bio

I'm in the W'14 batch at Hacker School, where I've worked on projects like creating sounds from spectrograms (huge failure) and replacing Python builtins and keywords with Harry Potter spells (huge success).

My background is in Theoretical Math. After college I optimized paid search ads for Adam & Eve and some other retailers (though my employer was Adlucent, an agency in Austin, TX). I then used scikit-learn to automate tasks like classification of search queries into product categories.

I will nerd out with you about programming, science fiction, feminism, comics, Dune (I <3 Dune. Dune, Dune, Dune.), math, board games, etc. I also think it's fabulous to drink champagne in bed.