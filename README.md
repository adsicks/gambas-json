# gambas-json
json tools for gambas

This is a JSON Explorer and Editor. It operates on the same basic principle of the Class Builder utility from early versions of VB. 

JSON files contain descriptions of JavaScript objects. So, we start out the file with a collection, an object, or a single value. If the first thing we encounter is a single value, then it is over. This is the only thing a JSON file can contain. If we start off with an object then we look for name, value pairs. The values can be collections, other objects, or single values. Again, at single values we return back to processing the rest of the object we are in. If it is an object we process the nested object recursively, the same way we are processing the current object. If we start off with a collection we look for a single value and object, or another collection. When we find a single value, we add it to the tree and continue. When we find an object or collection we recursively process them just like we entered. We process the collection to the end of the collection. This is a big exercise in recursion.

So, we have Collections of objects, Arrays of single values, Objects, or simply a single value. We can display and manipulate these with a ColumnView control. This will let us see visually the hierarchy of the collections and classes and easily give us a cursor to use to add members to Arrays, Collections, and objects. 

The possible columns will be Name, Value, Type, Parent, Full Path, Raw Text, Hexadecimal Representation, and binary representation. The value displayed will always be the unescaped string. The value entered will need to be an escaped string which will be processed upon entry to display unescaped.  Thus, the Raw Text field is needed to view escape characters. The Hex and binary fields are for debugging purposes and will show the raw representation of the current member same as the raw text. 

This is a work in process, but this is a needed tool for some of the web development I am undertaking. This is a convenience tool.
You can contact me with questions or comments, or if you want to add to this tool. My email is sales at zwebusa.com.
