
# Errors

In general, when you try to get a value from an invalid request, the attribute will return **None**

You can prevent this by adding a `isvalid` check before outputting.


```py
from stat5b5t import api, tools

stats = api.Statistics()
tests = tools.Debugging()

r = stats.request("uuid here")

if tests.isvalid(r) == True: # Checks if the given request (r) is valid
    do something #your code goes here
else:
    print("Something went wrong")
```

If  you don't know what exactly went wrong you can look at the raw response with
> `stats.raw(r)`

Another way to check this is by adding a feature that will output the error message like this

```py
from stat5b5t import api, tools

stats = api.Statistics()
tests = tools.Debugging()

r = stats.request("uuid here")

if tests.isvalid(r) == True:
    do something
else:
    print("Something went wrong")
    print(tests.errmsg(r))
```
