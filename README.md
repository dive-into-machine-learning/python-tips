# Get the Hang of Python

Hi! You're a beginner or intermediate, or even advanced. You want to learn mroe Python. There's so much out there: do not fret. This is a curated list of resources. I've picked and chosen. And you should go ahead and pick and choose further :)

I agree with [_Learn Ruby the Hard Way_](https://learnrubythehardway.org/book/preface.html) that the "hard way" — learning by doing — diving right in — is actually the easy way. So no matter your background, newbie programmer or advanced Pythonista, take a look and learn something new.

## Starters

The first key is Don't Panic. You can learn most by hacking. 

If you have not installed Python yet, you need to pick a version of Python and then install. For both of these subjects, you should read [_Hitchhiker's Guide to Python_](http://docs.python-guide.org/en/latest/). 

It's also a good idea to debunk the myths you may have heard about Python.

* [PayPal Engineering Blog: 10 Myths of Enterprise Python](https://www.paypal-engineering.com/2014/12/10/10-myths-of-enterprise-python/) (5-10 minute read)  
* (And more testimonies: [https://www.python.org/success-stories/](https://www.python.org/success-stories/)

![](http://imgs.xkcd.com/comics/python.png)

### Python community

If nobody’s told you yet, Python’s community is one of the most important things about it :) Join forums, subreddits ([/r/Python](https://reddit.com/r/Python), [/r/learnpython](https://reddit.com/r/Python)), chats (Slacks or [IRCs](http://webchat.freenode.net/?channel=%23%23learnpython)) local [meetups](https://meetup.com), etc., and get support. You’ll learn much better with a community.

### Cheat sheets/quickstarts

Keep these handy.

 * The official docs! [https://docs.python.org/2/](https://docs.python.org/2/)
 * [Learn X in Y Minutes: Python](https://learnxinyminutes.com/docs/python/) is a good cheat sheet.
 * [Flow-chart to help you get past common Python error messages](http://i.imgur.com/WRuJV6r.png)


### Courses and books

If you like self-guided courses, try one of these:

 * [RealPython](https://realpython.com/): "Real Python teaches programming and web development through hands-on, interesting examples that are useful and fun!" (paid)
 * or _[Dive into Python](http://www.diveinto.org/python3/)_ (the classic). (Note that [Dive into Python 3](http://www.diveinto.org/python3/) only covers new & advanced features in Python 3 - not the language as a whole. Don't start there.) (free)
 * or [Google's Python Introduction course (free)](https://developers.google.com/edu/python/)
 * or [How to Think Like a Computer Scientist: Learning with Python, Interactive Edition (free)](http://interactivepython.org/courselib/static/thinkcspy/index.html) — **if you're relatively new to programing, this is an especially good fit for you**

If you like taking online courses with a group, I’ve heard this one is good:

 * [Coursera: An Introduction to Interactive Programming in Python (free)](https://www.coursera.org/learn/interactive-python-1)

### A good IDE will help you be more productive!

A lot of people think when you're first learning a language like Python, you'll grok it best if you use a basic text editor instead of an IDE. Still, maybe you are just here to learn a little Python for some projects at work, and you just need to get some things done. An IDE might help you.

 * I strongly prefer JetBrains [PyCharm](https://www.jetbrains.com/pycharm/). So do most people at my company now. And many many people the world over … PyCharm does incredible things with your Python code. 
 * There's [a free Community Edition you can use immediately](https://www.jetbrains.com/pycharm/download/). We have Professional Edition licenses, so get your hands on one of those as soon as you can!
 
(Another side note on text editors vs. IDEs. Even if you like the lean text editor side of things ([vim](http://vim-adventures.com/) or Emacs, Sublime Text...) Well, I still think you should check out PyCharm. I hated disliked IDEs for a long time until I tried PyCharm...)

### Interactive tools for understanding Python better

Please try at least one of these out. Interactive tools can really deepen your understanding and accelerate your learning. A huge strength of Python is its interactivity ... Use it! 

 * "[Python Tutor](http://pythontutor.com/visualize.html), created by [Philip Guo](http://www.pgbovine.net/), helps people overcome a fundamental barrier to learning programming: understanding what happens as the computer executes each line of a program's source code."
  * It's amazing.
  * It’s also not just Python. Various languages supported
 * [ipython and ipython notebook - my own notes on it - you should be using these!!!](https://docs.google.com/document/d/1B-pK6Kt5AlgJ-mal_p4Bu9_-KJBys9hAALtwOm-LG7Q/pub) 
 * Use PyCharm's debugger, it is excellent. [JetBrains PyCharm docs: Debugging](https://www.jetbrains.com/pycharm/help/debugging.html)

### Avoiding common mistakes and pitfalls

Free book (PDF): [How to make mistakes in Python](http://www.oreilly.com/programming/free/files/how-to-make-mistakes-in-python.pdf)

### Testing

One of Python's biggest strengths is its testability. Test-Driven Development and Python go together happily.

  1. start with this concise post, [http://docs.python-guide.org/en/latest/writing/tests/#the-basics](http://docs.python-guide.org/en/latest/writing/tests/%23the-basics)
  2. then try this comprehensive post. It's about unit testing with Python's Standard Library unit test package, but leads you up to introducing pytest — the best runner for any kind of tests (you can get started on that right away). It’s also the best framework for writing data-driven tests, when you’re ready to get gung-ho about testing your code :D
  3. [Jeff Knupp: Improve your Python Understanding - Unit Testing](https://www.jeffknupp.com/blog/2013/12/09/improve-your-python-understanding-unit-testing/)
  4. When you’re ready, move onto pytest, definitely :) [pytest.md](pytest.md)

## For intermediate and advanced Pythonistas

Are you intermediate or advanced? If you're not sure, one way to check:

  * Ask yourself [Python Interview Questions](https://www.reddit.com/r/Python/comments/1knw7z/python_interview_questions) and see if you know them. If you don't, try and learn more
  * Read some of ["Good to Great Python Reads"](http://jessenoller.com/good-to-great-python-reads/), a nice index of great Python reading (good to Ctrl+F for topics)

### Style guides

You don’t need to read style guides until you’re beyond beginner status. At some point that will become very valuable and helpful to you :)

There are two main style guides:

1. [The Hitchhiker's Guide to Python](http://docs.python-guide.org/en/latest/) – opinionated guide by the legendary Kenneth Reitz of [requests](https://github.com/kennethreitz/requests]) fame
2. [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html) – perhaps the most widely-used Python style guide

### Special topics

Not comprehensive, but when I brain-dumped some really good things to know about, I wrote down these subjects.

- Unicode is pretty sad in Python 2, so if you're using Python 2 you should learn the gotchas and fixes ASAP...
 - [Unicode in Python, completely demystified](http://farmdev.com/talks/unicode/) (weird presentation format, but, you just press spacebar to proceed through slides)
 - [unicode frustrations](https://pythonhosted.org/kitchen/unicode-frustrations.html)  
- Functional programming, list comprehensions, etc.
 - [Python List Comprehensions: Explained Visually](http://treyhunner.com/2015/12/python-list-comprehensions-now-in-color/)
 - [Decorators & functional Python](http://brianholdefehr.com/decorators-and-functional-python)

- Security, with this bent: learning general skills to get into InfoSec or AppSecz
 - Step 1, listen to this: [Talk Python to Me #37: Python, Cybersecurity, and Penetration Testing](https://talkpython.fm/episodes/show/37/python-cybersecurity-and-penetration-testing) 
 - Step 2, read [Gray Hat Python (book 1/2)](http://www.amazon.com/Gray-Hat-Python-Programming-Engineers/dp/1593271921)  and/or [Black Hat Python (book 2/2)](http://www.amazon.com/gp/product/1593275900/])
 - [MartinFowler.com: "Web Security Basics" (regardless of programming language)](http://martinfowler.com/articles/web-security-basics.html)
- Machine Learning! Here’s my guide:  [Dive into Machine Learning](https://github.com/hangtwenty/dive-into-machine-learning) 


#### Scenario guide

You're probably going to use libraries to do a lot of things. When you have a new scenario and you are thinking what should I use... You should:

1. Ask your community :D
2. check [Hitchhiker's Guide to Python: Scenario Guide for Python Applications](http://docs.python-guide.org/en/latest/%23scenario-guide-for-python-applications)
3. check [Full Stack Python](http://www.fullstackpython.com/table-of-contents.html), another comprehensive but carefully curated guide, full of useful context, advice, etc.
4. check [Awesome Python](https://github.com/vinta/awesome-python), "A curated list of awesome Python frameworks, libraries, software and resources" — or the [Pythonidae](https://github.com/svaksha/pythonidae)  list

### Fast and scalable Python

#### Concurrency

For completely out-of-the-box Python, concurrency is slightly complicated (because of the GIL). However, it's not some no-man's-land or something. You don't need to rediscover the solution on your own. The best single summary I've seen of (preferred) concurrency options – 

[Myth: Python Lacks Concurrency](https://www.paypal-engineering.com/2014/12/10/10-myths-of-enterprise-python/%23python-lacks-concurrency)

but also, is concurrency exactly what you want? Maybe it is, but maybe a worker-and-queue option is more like what you want...

#### Parallelism/ distributed task queue

For Python projects that need some horizontal scale-out and fast performance, there's a good chance a worker-and-queue setup might work better for you, compared with single-computer concurrency. There's no question: Celery is the way to go for worker-and-queue systems in Python --

[Celery](http://docs.celeryproject.org/en/latest/)

#### Map/Reduce and beyond (Functional Reactive Programming)

Or maybe not worker-and-queue. I've maintained some pretty iffy worker-and-queue systems. These days I reach for [Apache Spark](http://spark.apache.org) instead. Batch and stream processing.
