# Online-Shopping-System---OOP-
    Authors: Ahmet Huseyin, Umut Ücük, Şemsi Belli

## Class "Item"

### Class Attributes:

#### Private:

- [x] ID (not set by user)
- [x] name
- [x] quantity
- [x] price

### Class Methods:

#### Public:

- [x] Default Constructor
- [x] Parameterized Constructor
- [x] Copy Constructor
- [x] Setters
- [x] Getters
- Operator Overloading
- [x] == (Equal if they have the same name)
- [x] += (Item's quantity will be increased by parameter item quantity)
- [x] -=
- [x] << (stream insertion operator) (print item)
- [x] > > (stream extraction operator)

- [x] Header for each function is added

---

## Class "Seller"

### Class Attributes:

#### Private:

- [x] name
- [x] email
- [x] items (dynamic array of objects of type **Item** with the size maxItems)
- [x] maxItems

### Class Methods:

#### Public:

- [x] Parameterized Constructor
- [x] Destructor
- Operator Overloading
- [x] << (stream insertion operator)
- _Add An Item_
- [x] Takes an **Item** object as a parameter
- [x] Function Body

  - (Use Operator == where an item is equal to another If They have the same name)
  - If the item exists Increase the item’s quantity by the quantity of the parameter item using the (+=) of **Item** class
  - And the price of the parameter object will be ignored
  - **Else :**
  - You will add it to the seller's items
  - **Return (boolean) :**
  - true if item addition was successful (If there is a place in the array)
  - false otherwise

- _Sell An Item_
- [x] Takes item name and quantity as parameters
- [x] If the parameter quantity <= item's quantity then decrease it from item using the (-=) of **Item** class
  - **Else :** (parameter quantity more than that of the item)
  - Print " There is only {item's quantity} left for this item "
  - **Return (boolean):**
  - true if the item was found
  - false otherwise
- _Print Items_
- [x] Print all the item info for the seller (print each item using << of **Item** class)

- _Find an Item by ID_
- [x] This returns an Item object (or a pointer to Item) with the specified ID if there is an item with such ID.

---

## Main Function

- [x] Ask Seller to input his detalis (seller's info)
- [x] Ask Seller for his store capacity (maxNumberOfItems)
- Menu To Choose from:
- [x] 1. Print My info (print seller's info using << of **Seller** class)
- [x] 2. Add an Item
- [x] 3. Sell an Item
- [x] 4. Print Items
- [x] 5. Find an Item by ID
- [x] 6. Exit

---

### Comments

- [x] Author and Purpose of the Program
- [x] For every function explaining what it does, Parameters it takes and return value
- [x] Add comments to any part that is difficult to understand

---

### Coding Style

#### Naming:

- [x] Names representing methods or functions are verbs and written in mixed case starting with lower case
- [x] Private class variables should have underscore suffix. ex: int length\_
- [x] Generic variables should have the same name as their type. ex: void setTopic(Topic\* topic)
- [x] Non-generic variables have a role. These variables can often be named by combining role and type ex1: Point startingPoint, centerPoint; ex2: Name loginName;
- [x] Variables with a large scope should have long names, variables with a small scope can have short names [1]
- [x] The name of the object is implicit, and should be avoided in a method name ex: line.getLength(); NOT: line.getLineLength();
- [x] Plural form should be used on names representing a collection of objects.
- [x] The prefix is should be used for boolean variables and methods. ex: isSet, isVisible, isFinished, isFound, isOpen
- [x] Negated boolean variable names must be avoided.
- [x] Abbreviations in names should be avoided.
- [x] Naming pointers specifically should be avoided. ex: Line* line; NOT: Line* pLine; NOT: Line\* linePtr;
- [x] C++ pointers and references should have their reference symbol next to the type rather than to the name ex1: float* x; NOT: float *x; ex2: int& y; NOT: int &y;

#### Position

- [x] Loop variables should be initialized immediately before the loop ex: isDone = false; while(){} NOT: bool isDone = false; while(){}
- [x] Complex conditional expressions must be avoided. Introduce temporary boolean variables instead
- [x] Executable statements in conditionals' conditions must be avoided.

#### Other Notes

- [x] Floating point constants should always be written with decimal point and at least one decimal
- [x] "0" should be used instead of "NULL". Note: NULL is part of the standard C library, but is made obsolete in C++.

#### Spaces

- [x] Commas should be followed by a white space
- [x] Operators should be surrounded by a space character.
- [x] C++ reserved words/function's name should be followed by a white space
- [x] Methods should be separated by three blank lines.
- [x] Use alignment wherever it enhances readability.

