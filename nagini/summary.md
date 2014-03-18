This is a talk that explores Python internals by attempting to replace the `import` keyword/statement with `accio`. I cover:

* how to access and easily remove/overwrite Python builtin functions interactively in a Python interpreter)

* what Python statements are, and why overwriting Python statements is hard (but overwriting Python builtin functions is easy)

* where to find the definitions of Python statements in the CPython source code (this is much less scary/overwhelming than it sounds, I promise! It's all in a very easy-to-read Grammar file.)

* why making changes to Python's Grammar and then recompiling doesn't always work (spoiler alert: it's because half of CPython is written in Python!), and how to use bootstrapping to work around this