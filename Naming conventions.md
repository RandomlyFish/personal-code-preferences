# Naming conventions

The purpose of the following guidelines are not to restrict what names you can use for variables and functions, but to make it easier to pick suitable names that will stay consistent with the other variables and functions in your code.

<br>

## Variable names

The core concept which applies to all the following guidelines is that the way a variable is named should make it obvious what the type of the variable is. This is especially important in a language like javascript, where you generally don't annotate the type of variables.

<br>

### booleans
* Should start with a verb, such as "is", "has", "can", "will" etc
* If the verb is left out, it should end with "ed" or "ing"

Examples: "isActive", "hasFinished", "canPlay", "willBeRemoved", "played", "playing", "completed"

<br>

### arrays
* Should end with "s" or another form of ending which implies that it can hold more than one value
* should not end with "Array"

"Array" in the name should be avoided as it will result in an inconsistent naming convention, unless all the array variables use that. An exception to this could of course be when it's a generic array used in a utility class for arrays.

Examples: "items", "highscores", "children"

<br>

### objects
 * should include a word which describes a collection of data
 
Examples: "animationOptions", "productDetails", "graphicSettings", "itemInfo"

<br>

## Variable name implications

Making sure that the name of a variable accurately represet what it stores is extremely important.

<br>

### Word order matters

Let's take two similar variable names as an example, "rectangleCenterPosition" and "centerRectanglePosition". Both contains the same words, with only the order of "rectangle" and "center" switched, yet the implication ends up being completely different.

* "rectangleCenterPosition" = The position at the center of the rectangle
* "centerRectanglePosition" = The rectangle which is in the center
