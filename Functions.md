# Functions

The purpose of the following guidelines are to make functions more predictable, and clear what they do simply by looking at the name of them.

<br>

## Function prefixes

### get
* Should only return existing infromation
* Should not modify values or state
* Should return the same value if called repeatedly (unless implied in the function name)

An example of a bad use of the get prefix, is a get function which removes a value from an array and returns it. Unless it's clearly implied in the function name, this is very likely to cause issues if the function is called in more than 1 place.

An example where the function could return different values each time would be a function like: "getRandomValue", where the name of the function implies that it won't return the same value each time.

<br>

### set
* Should take a value passed to the function and overwrite an existing value

<br>

### offset
* Should take a value passed to the function and add it to an existing value

The value should always be added to the existing value, never subtracted. If you need to offset something with a negative value, the offset value itself should be negative. This is important as it makes each offset function work the same way.

<br>

### configure
* Should take an object passed to the function and modify existing values based on the passed object

<br>

### fetch/request
* Should be an asynchronous get function which eventually returns a value

<br>

### create
* Should only create objects or instances of classes and return them

<br>

### add
* Should create objects or instances of classes and add them to something, such as an array
* Should return what it created

<br>

## Responsibilities

Functions should have as few responsibilites as they can, while still providing enough useful functionality. A good rule of thumb is if you can't come up with short name that accurately represent what the function does, it probably does too much.

Along with good use of prefixes, you should be able to look at the name of a function and know more or less what it will do.
