---
layout: post
title: Import Libraries Automatically in IPython
---

I use IPython quite often in everyday work. So it would be handy if IPython
could import some libraries automatically.

For scientific computing, perhaps the most popular option for IPython is
`--pylab`
which imports numpy and matplotlib automatically. Check the below example.

![pylab example]({{ site.baseurl }}/images/pylab.png "IPython --pylab example")

Another way to import libraries when starting IPython is to create a startup
file for python. I created a python file called `.startup.py` which contains the
below codes in it.

```python
print("load ~/.startup.py")
print("import sys, collections, functools, itertools, heapq, pprint, bisect, operator, math")
import sys, collections, functools, itertools, heapq, pprint, bisect, operator, math
pp = pprint.pprint
```

Also I set the enviornment variable **PYTHONSTARTUP** through puting the below
line in `.bashrc` file.

```bash
export PYTHONSTARTUP=~/.startup.py
```

Enjoy your IPython.

![startup example]({{ site.baseurl }}/images/startuppy.png "IPython startup example")


