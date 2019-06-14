No Python documentation found for 'beats.ipynb'.
Use help() to get the interactive help utility.
Use help(str) for help on the str class.

Attribute references
********************

An attribute reference is a primary followed by a period and a name:

   attributeref ::= primary "." identifier

The primary must evaluate to an object of a type that supports
attribute references, which most objects do.  This object is then
asked to produce the attribute whose name is the identifier.  This
production can be customized by overriding the "__getattr__()" method.
If this attribute is not available, the exception "AttributeError" is
raised.  Otherwise, the type and value of the object produced is
determined by the object.  Multiple evaluations of the same attribute
reference may yield different objects.

Related help topics: getattr, hasattr, setattr, ATTRIBUTEMETHODS, FLOAT,
MODULES, OBJECTS

