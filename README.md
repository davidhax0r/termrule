termrule
========

Tired of destroying the Enter key by creating a "void zone" in your terminal so that you can see the error that you're trying to debug? If yes, this is for you. `termrule` allows you to create colored horizontal rule in terminal. Use it in place of the old `<hr />` tag in terminal. This script is inspired from hr.py by euangoddard.

### Installation
` $ pip install termrule `

### Usage
#### Command Line
```
usage: hr [-h] [--color COLOR] symbol [symbol ...]

positional arguments:
  symbol         Symbol for horizontal line

optional arguments:
  -h, --help     show this help message and exit
  --color COLOR  Color of the line
```
```
$ hr "#"
#################################### # Till the end of terminal 

$ hr "#-#"
#-##-##-##-##-##-##-##-##-##-##-##- # Till the end of termnial 

$ hr "@" --color red
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@ # Till the end of terminal in red color
```

#### Script
```python
>>> from tr import TermRule
>>> r = TermRule()
>>> r.hr(["#", "-"], color="cyan")
##################################### # Till the end of terminal in cyan color
-------------------------------------
>>> r.hr(["^"])
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ # Till the end of terminal in default color
```

### Dependencies
termcolor is the only dependency; it is used for colored outputs

### License
termrule is distributed under MIT license, see LICENSE for more details
