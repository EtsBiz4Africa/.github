# Odoo developpers cheatsheet
This contains some codes excerpts helpful while developping or troubleshooting Odoo ERP instance.

## Debugging
### whilingly printing backtrace at certain point
```
import traceback

def do_stuff():
    raise Exception("test exception")

try:
    do_stuff()
except Exception:
    print(traceback.format_exc())
```
[Source](https://stackoverflow.com/a/3702847)
