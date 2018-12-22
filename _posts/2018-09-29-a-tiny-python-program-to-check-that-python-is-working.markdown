---
title: A tiny Python program to check that Python is working
date: 2018-09-29 16:27:00 Z
layout: post
categories:
- PYTHON
---

A tiny Python program to check that Python is working.
Try running this program from the command line like this:

```
python hello.py
python hello.py Alice
```

That should print:

```
Hello World -or- Hello Alice
```

Try changing the 'Hello' to 'Howdy' and run again. Once you have that working, you're ready for class -- you can edit and run Python code; now you just need to learn Python!

```python
import sys

# Define a main() function that prints a little greeting.

def main():

# Get the name from the command line, using 'World' as a fallback.

if len(sys.argv) >= 2:
name = sys.argv[1]
else:
name = 'World'
print 'Hello', name

# This is the standard boilerplate that calls the main() function.

if **name** == '**main**':
main()
```
