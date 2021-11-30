
# [5b5t statistics](https://github.com/ScobraScope/stats5b5t)
API wrapper for 5b5t's statistics

[**THIS IS JUST THE DOCUMENTATION REPO. THE LIBRARY REPO CAN BE FOUND HERE**](https://github.com/ScobraScope/stats5b5t)

```pip install stats5b5t```

> **Tested on: [Python 3.9](https://www.python.org/downloads/release/python-390)**

## Documentation
Click on the modules to be taken to the detailed Documentation

**Modules:**
    [**api,**](https://github.com/ScobraScope/stats5b5t-documentation/blob/main/doc/api.md)
    [**tools,**](https://github.com/ScobraScope/stats5b5t-documentation/blob/main/doc/tools.md)
    [**errors**](https://github.com/ScobraScope/stats5b5t-documentation/blob/main/doc/errors.md)
## Usage
```py
from stats5b5t import api

stats = api.Statistics()

r = stats.request("uuid here")

print(stats.kills(r))
```

**With debugging:**

```py
from stat5b5t import api, tools

stats = api.Statistics()
tests = tools.Debugging()

r = stats.request("uuid here")

print(stats.kills(r))
print(tests.isvalid(r))
print(tests.missmatch(r))
print(tests.errmsg(r))
```

## Modules: api, tools

> **api**

Handles requests and data sorting for you.

> **tools**

Handles debugging and checks for you.


