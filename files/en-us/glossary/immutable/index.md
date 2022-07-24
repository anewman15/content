---
title: Immutable
slug: Glossary/Immutable
tags:
  - CodingScripting
  - Glossary
---
An immutable {{glossary("object")}} is one whose content cannot be changed.
An object can be immutable for various reasons, for example:

- To improve performance (no planning for the object's future changes)
- To reduce memory use (make {{glossary("object reference","object references")}} instead of cloning the whole object)
- Thread-safety (multiple threads can reference the same object without interfering with one other)

Strings and Numbers are Immutable. Lets understand this with an example:

var immutableString = "Hello";

// In the above code, a new object with string value is created.

immutableString = immutableString + "World";

// We are now appending "World" to the existing value.
Copy to Clipboard
On appending the "immutableString" with a string value, following events occur:

Existing value of "immutableString" is retrieved
"World" is appended to the existing value of "immutableString"
The resultant value is then allocated to a new block of memory
"immutableString" object now points to the newly created memory space
Previously created memory space is now available for garbage collection.

## See also

- {{interwiki("wikipedia", "Immutable object", "Immutable")}} on Wikipedia
