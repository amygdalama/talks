Some things we will learn:

 - What is a `SyntaxError`?
 - How does the Python interpreter know if something is a `SyntaxError`?
 - What does it mean for a line of code to be a valid Python statement?



Goal: We want to rename "import" with something more aethestically satisfying / edifying / fun / groovy / …

1.  Redefining many statements is done in the "Grammar" file, which defines an inventory of legal statements in the language.
2.  Naive first effort: replace literal strings in the Grammar file, changing 'import' => 'accio'
a.  error; reason is that Python's codebase is in two parts: one C, one Python
b.  simplified explanation: The Python part of the codebase already contains 'import', so 'import' cannot be removed completely.
3.  Second effort: replace 'import' => 'accio' also in those Python scripts residing in the Cpython sourcecode
a.  error; some of these Python scripts are being executed by your computer's environment Python
4.  Third effort: replacement requires two steps;
a.  first create an interim version of Python in which 'import' and 'accio' coexist, and use that as the  environment Python;
b.  after that, clone CPython again, this time removing 'import'
c.  After compilation of this second version, bingo!

Summary:
    to rename "import", you do two cycles of editing the Grammar file and recompiling the language

——————

other fun stuff, perhaps in one (or more) separate slide-sets

