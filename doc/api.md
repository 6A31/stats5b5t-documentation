
# api

```py
stats = api.Statistics()
```

**All attributes work with a request variable.**
**Make sure to pass the request with each attribute like shown below.**


## Attributes

**Format:**
This is a basic showcase with placeholders
```py
stats = api.Statistics()

r = stats.request("uuid here") # Make the api call and define it as "r"

stats.attribute(r) # Pass the variable "r" to your "attribute"
```
 
### Attributes / Functions

**Base:**
> stats.x(y)

x = attribute
y = request

> raw(y)
Returns the raw JSON string from the api call.

> uuid(y)
Returns the UUID of the requested profile.

> ratio(y)
Returns the Kill / Death ratio of the requested profile.

> kills(y)
Returns the Kills of the requested profile.

> deaths(y)
Returns the Deaths of the requested profile.

> joindate(y)
Returns the Joindate of the requested profile.
Returned value: str Text

> lastplayed(y)
Returns the time the requested profile was last seen online.
Returned value: str Text

> leaves(y)
Returns the amount of times a user has left the server.

> enderpearls(y)
Returns the amount of enderpearls a user has thrown.

> crystal(y)
Returns the amount of crystals a user has placed.

> damage(y)
Returns the amount of damage a user has given

> damagetaken(y)
Returns the amount of damage a user has taken.

> mobkills(y)
Returns the amount of mobs that a user has killed.

> jumps(y)
Returns the amount of times a user jumped.

> timesincedeath(y)
Returns the amount of time that has passed since the user was last killed.
Returned value: Ticks.
20 Ticks = 1 second. Divide all ticks by 20 to get seconds

> score(y)
Returns a user's score.

> healt(y)
Returns a user's health from the last time he logged out.

> platime(y)
Returns a user's playtime.
Returned value: Ticks.
20 Ticks = 1 second. Divide all ticks by 20 to get seconds

> recordtime(y)
Returns the time this data was taken.
Returned value: str Text

