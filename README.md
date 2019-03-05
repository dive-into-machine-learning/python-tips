# Learn More Python

Hi! Your skill level is beginner or intermediate, or even advanced. You want to [learn][1] more Python. There are plenty of resources out there, and this is just a curated list of links. Some for each skill level. It's not everything and the kitchen sink, but it's not all "must-read" either. You should feel free to skip around.

A note on approach: I agree with [_Learn X the Hard Way_](https://learnpythonthehardway.org/book/preface.html) that [the "hard way" — learning by doing — diving right in — is actually the easy way.][1] So new or not, let's jump in.

## Starters

The first key is Don't Panic. You can learn most [by hands-on experience][1]. A significant benefit of a language like Python, is how learnable it is by jumping into an interactive session. Rapid feedback.

If you have not installed Python yet, you need to pick a version of Python and then install. For both of these subjects, you should read [_Hitchhiker's Guide to Python_](http://docs.python-guide.org/en/latest/). **UPDATE in 2019:** start with Python 3!

[1]: (https://github.com/hangtwenty/python-is-for-lovers/issues/15)

**It's also a good idea to debunk the myths you may have heard about Python:**

* **[PayPal Engineering Blog: 10 Myths of Enterprise Python](https://www.paypal-engineering.com/2014/12/10/10-myths-of-enterprise-python/) -- read this post whether are new to Python or not. It's great, and useful.**   


As for _why_ to learn it (and ignore the bellyachers who are wasting their time telling you what to learn): 

* [python.org → "Success Stories"](https://www.python.org/success-stories/)
* [this Quora thread on _some_ other famous cases](https://www.quora.com/What-top-tier-companies-use-Python)
* [this more general Quora thread about why dynamic languages are found in startups and innovative environments](https://www.quora.com/Why-do-startups-always-use-slow-language-such-as-Python-and-Ruby-but-large-company-uses-fast-language-like-C++-Java-and-Scala). Remember, you are not saying no to other languages. You are just equipping yourself with more. And it's _fun_ god-dammit.)

![](http://imgs.xkcd.com/comics/python.png)

### Python community

If nobody’s told you yet, Python’s community is one of the most important things about it :) Join forums, subreddits ([/r/Python](https://reddit.com/r/Python), [/r/learnpython](https://reddit.com/r/Python)), chats (Slacks or [IRCs](http://webchat.freenode.net/?channel=##learnpython)) local [meetups](https://meetup.com), etc., and get support. You’ll learn much better with a community.

### Cheat sheets/quickstarts

Keep these handy.

 * The official docs! [https://docs.python.org/2/](https://docs.python.org/2/)
 * [Learn X in Y Minutes: Python](https://learnxinyminutes.com/docs/python/) is a good cheat sheet.
 * [Flow-chart to help you get past common Python error messages](http://i.imgur.com/WRuJV6r.png)


### Courses and books

If you like self-guided courses, try one of these:

 * [_Learn Python the Hard Way_](https://learnpythonthehardway.org/)
 * [RealPython](https://realpython.com/): "Real Python teaches programming and web development through hands-on, interesting examples that are useful and fun!" (paid)
 * or _[Dive into Python](http://www.diveintopython.net/)_ (the classic). (Note that [Dive into Python 3](http://www.diveintopython3.net/) only covers new & advanced features in Python 3 - not the language as a whole. Don't start there if you're new to Python) (free)
 * or [Google's Python Introduction course (free)](https://developers.google.com/edu/python/)
 * or [How to Think Like a Computer Scientist: Learning with Python, Interactive Edition (free)](http://interactivepython.org/courselib/static/thinkcspy/index.html) — **if you're relatively new to programing, this is an especially good fit for you**

If you like taking online courses with a group, I’ve heard this one is good:

 * [Coursera: An Introduction to Interactive Programming in Python (free)](https://www.coursera.org/learn/interactive-python-1)

### A good IDE will help you be more productive!

A lot of people think when you're first learning a language like Python, you'll grok it best if you use a basic text editor instead of an IDE. Still, maybe you are just here to learn a little Python for some projects at work, and you just need to get some things done. An IDE might help you.

 * I strongly prefer JetBrains [PyCharm](https://www.jetbrains.com/pycharm/). So do most people at my company now. And many many people the world over … PyCharm does incredible things with your Python code. 
 * There's [a free Community Edition you can use immediately](https://www.jetbrains.com/pycharm/download/).
 
(Another side note on text editors vs. IDEs. Even if you like the lean text editor side of things - [vim](http://vim-adventures.com/) or Emacs, Sublime Text... Well, I still think you should check out PyCharm. I hated disliked IDEs for a long time until I tried PyCharm. Vim users, take a look at ["Epic Review of PyCharm [...] From a Vim User's Perspective"](https://andrewbrookins.com/tech/one-year-later-an-epic-review-of-pycharm-2-7-from-a-vim-users-perspective-older2/) (and ["Part 2"](https://andrewbrookins.com/tech/one-year-later-an-epic-review-of-pycharm-2-7-from-a-vim-users-perspective/). The vim emulation is solid, I use it every day.)

### Interactive tools for understanding Python better

 * [ipython and ipython notebook - you should be using these!!!](https://docs.google.com/document/d/1B-pK6Kt5AlgJ-mal_p4Bu9_-KJBys9hAALtwOm-LG7Q/pub) 
 * There's also Python's built-in debugger, `pdb`, and the ipython variant (autocomplete etc) [`ipdb`](https://github.com/gotcha/ipdb)
 * Use PyCharm's debugger, it is excellent. [JetBrains PyCharm docs: Debugging](https://www.jetbrains.com/pycharm/help/debugging.html)

### Avoiding common mistakes and pitfalls

Free book (PDF): [How to make mistakes in Python](http://www.oreilly.com/programming/free/files/how-to-make-mistakes-in-python.pdf)

### Testing

One of Python's biggest strengths is its testability. Test-Driven Development and Python go together happily.

  1. start with this concise post, [http://docs.python-guide.org/en/latest/writing/tests/#the-basics](http://docs.python-guide.org/en/latest/writing/tests/#the-basics)
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

- Security, with this bent: learning general skills to get into InfoSec or AppSec
    - Step 1, listen to this: [Talk Python to Me #37: Python, Cybersecurity, and Penetration Testing](https://talkpython.fm/episodes/show/37/python-cybersecurity-and-penetration-testing) 
    - Step 2, read [Gray Hat Python (book 1/2)](http://www.amazon.com/Gray-Hat-Python-Programming-Engineers/dp/1593271921)  and/or [Black Hat Python (book 2/2)](http://www.amazon.com/gp/product/1593275900/])
    - [MartinFowler.com: "Web Security Basics" (regardless of programming language)](http://martinfowler.com/articles/web-security-basics.html)
- Machine Learning! Here’s my guide:  [Dive into Machine Learning](https://github.com/hangtwenty/dive-into-machine-learning) 


#### Scenario guide

You're probably going to use libraries to do a lot of things. When you have a new scenario and you are thinking what should I use... You should:

1. Ask your community :D
2. check [Hitchhiker's Guide to Python: Scenario Guide for Python Applications](http://docs.python-guide.org/en/latest/#scenario-guide-for-python-applications)
3. check [Full Stack Python](http://www.fullstackpython.com/table-of-contents.html), another comprehensive but carefully curated guide, full of useful context, advice, etc.
4. check [Awesome Python](https://github.com/vinta/awesome-python), "A curated list of awesome Python frameworks, libraries, software and resources" — or the [Pythonidae](https://github.com/svaksha/pythonidae)  list

### Fast and scalable Python - Concurrency, Parallelism

#### Nice cheat sheet on various non-beginner topics in Python 3

https://www.pythonsheets.com/

#### Concurrency?

For completely out-of-the-box Python, concurrency is slightly complicated (because of the [GIL](https://wiki.python.org/moin/GlobalInterpreterLock)). However, it's not some no-man's-land or something. You don't need to rediscover the solution on your own. The best single summary I've seen of (preferred) concurrency options – 

[Myth: Python Lacks Concurrency](https://www.paypal-engineering.com/2014/12/10/10-myths-of-enterprise-python/#python-lacks-concurrency)

There are loads of options... Greenlet, Twisted. I must say, while I've used those, I tend to go for parallelism with Celery if it makes sense. While it's a different solution, it can be relevant to some of the same problems you might be trying to solve.

#### Parallelism/ distributed task queue

For Python projects that need some horizontal scale-out and fast performance, there's a good chance a worker-and-queue setup might work better for you, compared with single-computer concurrency. There's no question: Celery is the way to go for worker-and-queue systems in Python --

[Celery](http://docs.celeryproject.org/en/latest/)

#### Map/Reduce and beyond (Functional Reactive Programming)

Or maybe not worker-and-queue. I've maintained some pretty iffy worker-and-queue systems. These days I reach for [Apache Spark](http://spark.apache.org) instead. Batch and stream processing, in a portable fashion, with a very declarative and maintainable API (thanks to [Functional Reactive Programming](https://gist.github.com/staltz/868e7e9bc2a7b8c1f754)).

## Further Reading

Use these links to further expand your knowledge base.

[r/LearnPython Wiki](https://www.reddit.com/r/learnpython/wiki/index) - Plethora of useful resources including video lectures, useful tools, and communities for learning competetive programming to keep you on an edge.

[Learn Python the Hard Way (Book)](https://learnpythonthehardway.org/book/) - This is an excellent beginner programmer’s guide to Python. It covers “hello world” from the console to the web.

[svaksha's python resources](https://github.com/svaksha/pythonidae/blob/master/Resources.md) - More books, a beginner's guide to Git, blog posts on Python/CS/Data Science, videos, and workshop tutorials.

[Hitchhikker's Guide to Python learning resources](http://docs.python-guide.org/en/latest/intro/learning/) - Links to good python books/guides. This book itself is a practical approach to learning Python. It assumes you already know the basics, and teaches you when & how to use Python. Read this book for a more example-driven approach.

[Think Like A Computer Scientist](http://interactivepython.org/runestone/static/thinkcspy/index.html) - Interactive python guide. Also includes programming a GUI, Recursion, Classes & Objects, and includes interesting game examples.

If you're coming from Java, you should [watch this](https://www.youtube.com/watch?v=OSGv2VnC0go) video for sure and/or grab [this ~70-page book](https://jeffknupp.com/writing-idiomatic-python-ebook/)

Writing a program and none of the guides/docs are helping out? Ask real programmers for help on [Stackoverflow](http://stackoverflow.com/documentation/python/topics) 
