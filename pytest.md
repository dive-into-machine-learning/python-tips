**UPDATE:** Your best source will be [this book on pytest](https://pragprog.com/book/bopytest/python-testing-with-pytest). Please bookmark that for later even if you read this little doc!

# py.test

py.test - running your existing tests! and also, how to write new tests with pytest

## New? Head to external documentation, first

pytest's documentation is excellent. Start there:

  * [Start with the official pytest documentation ](http://pytest.org/) Peruse it. Bookmark it. Refer to it frequently.

I would also recommend reading the Hitchhiker's Guide to Python sections on Testing:

  * [Testing Your Code](http://docs.python-guide.org/en/latest/writing/tests/)
  1. [The Basics](http://docs.python-guide.org/en/latest/writing/tests/%23the-basics)
  2. [Tools](http://docs.python-guide.org/en/latest/writing/tests/%23tools)

## Tips re: running tests with pytest

### Installation

```
pip install pytest
```

You run tests with pytest even if you are using unittest or nosetest in your suite. The pytest runner is great in itself... There's no reason to deprive yourself of the great benefits the pytest test runner offers.


### Usage and invocations

For historical reasons, the command is py.test. Not 'pytest.' Feel free to alias this if it bugs you. (`echo "alias pytest=py.test" >> ~/.bashrc`)

The [official documentation on usage and invocations](http://pytest.org/latest/usage.html%23usage) is excellent. Check it out!

Must specially call out this excellent feature:

```
-l, --showlocals    #  show [values of all] locals in tracebacks (disabled by default).
```

### Using pdb in conjunction with py.test

In many cases, you'd want to drop into pdb (Python's built-in debugger) in order to explore values of different variables at a certain point in your code. Usually to figure out what's going wrong. Well, py.tests --showlocals option will already take care of that for you, so you don't need to do that anymore.

If, however, you want to drop into pdb so you can actually interact, py.test makes it easy. There are two ways to do it. First, just call py.test with the --pdb argument:

```
py.test spam.py --pdb
```

However, if you're writing a browser test, and the failure is actually an assertion failure, you may already be past the point where the browser is automatically quit, by the time you drop into pdb. That's not great, because then you can't interact with the browser, which you might need to do. So if you need more control, just insert the following line, at the point where you want to drop into pdb; typically, the line above whatever line is causing your problem.

```
import pytest; pytest.set_trace()
```

Lastly, note that you can also use ipython's suped-up debugger ipdb if you'd like. Drop the regular ipdb.set_trace function in your code:

    import ipdb; ipdb.set_trace()

Now you'll have to run py.test with the -s/--capture=no option.
 
    py.test spam.py --capture=no

    py.test spam.py -s  # for short

And debug away.


### Integration with your IDE

#### PyCharm integration

PyCharm has very good native support for py.test. See the [official documentation](http://www.jetbrains.com/pycharm/webhelp/run-debug-configuration-py-test.html).

#### Eclipse PyDev integration

See the external document here: [Eclipse PyDev integration](http://pydev.org/manual_adv_pyunit.html).

----

# Writing tests with pytest

## Essential differences from stdlib's unittest

### Getting started

The basic introduction to py.test explains a lot. One of the things you'll notice immediately is that py.test tests don't have to be wrapped in the weird (pseudo-)classes that conventional Python tests make you use.

[Get Started](http://pytest.org/latest/getting-started.html%23getstarted) with py.test (official documentation)

### Assertions

#### Pythonic assertions with assert

pytest supports true python assert statements (it's a mystery why the stdlib package doesn't!). In the event of an assertion failure, pytest inspects the assertion and gives you all sorts of great information appropriate to the type of comparison you're evaluating.[pytest does awesome reporting in general](http://pytest.org/latest/example/reportingdemo.html%23tbreportdemo), for example showing you a diff between two collections:

```
failure_demo.py:69: AssertionError
_________________ TestSpecialisedExplanations.test_eq_set __________________

 

    self = <failure_demo.TestSpecialisedExplanations object at 0x1434310>

        def test_eq_set(self):
    >       assert set([0, 10, 11, 12]) == set([0, 20, 21])
    E       assert set([0, 10, 11, 12]) == set([0, 20, 21])
    E             Extra items in the left set:
    E         10
    E         11
    E         12
    E             Extra items in the right set:

    E         20

    E         21
```

#### Making assertions about exceptions with pytest.raises

pytest is compatible with stdlib's unittest. It plays just fine with the methods on unittest.TestCase like assertEquals and so on, so you don't need to go back through old tests and change those.

There is one special context to note. If you want to assert that executing some code will raise a certain kind of exception, use pytest.raises ([pytest docs: pytest.raises](http://pytest.org/latest/assert.html%23assertions-about-expected-exceptions)). It uses a context manager (with...) and it looks like this:

Asserting that an exception is raised

    import pytest

    with pytest.raises(ZeroDivisionError):
        1 / 0

Places where you used to use unittest.TestCase's assertRaises method may need to be updated to pytest.raises, not sure.

#### Documentation

  * [pytest docs: Asserting with the assert statement](http://pytest.org/latest/assert.html)
  * [pytest docs: pytest.raises](http://pytest.org/latest/assert.html%23assertions-about-expected-exceptions) (replacement for unittest.TestCase.assertRaises)
  * [Python docs: assert](http://docs.python.org/2/reference/simple_stmts.html%23the-assert-statement)

## Use parametrize, it's a game changer

  * py.test
  *  doctests ([official Python documentation](https://docs.python.org/2/library/doctest.html), [official py.test documentation](http://pytest.org/latest/doctest.html)
  * py.test's parametrize feature ([official documentation](http://pytest.org/latest/parametrize.html%23pytest-mark-parametrize)) [ed: parameterize is a valid English spelling too ...]
  * py.test's fixture feature ([official documentation](http://pytest.org/latest/fixture.html))

# Troubleshooting note

There’s some integration between pytest and tox. You’ll often use them together. Always use tox’s configuration files. Pytest will work with them. Tox will work with them. You’ll have confusion otherwise :)

TIP: ONLY use a tox.ini. If you have a pytest.ini, move the bits under the [pytest] section into a [pytest] section in your tox.ini. Do the same for setup.cfg if you have one.

Or expect confusion, sooner or later!

[http://pytest.org/latest/customize.html](http://pytest.org/latest/customize.html)

tox.ini can handle all your needs, and it is the simplest solution that will work with the most tools.
