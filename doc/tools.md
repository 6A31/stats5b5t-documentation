
# tools

```py
tests = tools.Debugging()
```

**All attributes work with a request variable.**
**Make sure to pass the request with each attribute like shown below.**


## Attributes

**Format:**
This is a basic showcase with placeholders
```py
stats = api.Statistics()
tests = tools.Debugging()
r = stats.request("uuid here") # Make the api call and define it as "r"
tests.attribute(r) # Pass the variable "r" to your "attribute"
```
 
### Attributes / Functions

**Base:**
> **stats.x(y)**

x = attribute
y = request

## isvalid

> **isvalid(y)**
Returns True or False based off if the api call was a success or not.

Example:

```json
{"err":"user does not exist"}
```

In this case, isvalid will return False

## missmatch

> **missmatch(y, x)**
Compares the API output and your input to confirm that the api returned the correct profile

Usage:
```py

tests.missmatch(y, expecteduuidhere)
```
This will return either True or False

## errmsg

> **errmsg(r)**
Returns the error message from the API

If the api does not return an error message, this will return:
`"No error message provided. JSON response is valid"`
If the api did return an error, it will return a string with the error message.

