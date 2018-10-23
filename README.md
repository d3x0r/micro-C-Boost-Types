# Micro C-Boost (no relation)

This is a family of amalgamated products from [SACK](https://www.github.com/d3x0r/sack).  

# Types

This is the smallest subset.  It includes most things 

This is a C file, but if the .h is included as C++ then namespaces will
be used, and the .c file should be renamed as .cc/.cpp/... or compiler option
otherwise forced to C++.

```
@set SRCS= %SRCS%   ../../src/typelib/typecode.c 
@set SRCS= %SRCS%   ../../src/typelib/text.c 
@set SRCS= %SRCS%   ../../src/typelib/input.c
@set SRCS= %SRCS%   ../../src/typelib/sets.c
@set SRCS= %SRCS%   ../../src/typelib/binarylist.c 
@set SRCS= %SRCS%   ../../src/typelib/url.c
@set SRCS= %SRCS%   ../../src/fractionlib/fractions.c
@set SRCS= %SRCS%   ../../src/memlib/sharemem.c 
@set SRCS= %SRCS%   ../../src/memlib/memory_operations.c 
@set SRCS= %SRCS%   ../../src/deadstart/deadstart_core.c 

// this requires file system fixes 
@set SRCS= %SRCS%   ../../src/vectlib/vectlib.c

```

An old build of the documentation (there haven't been a LOT of updates)
http://sack.sf.net
[containers](http://sack.sourceforge.net/sack__containers.html)

- [General](http://sack.sourceforge.net/sack.html)
- [Memory](http://sack.sourceforge.net/sack__memory.html)


- [containers](http://sack.sourceforge.net/sack__containers.html) - threadsafe
  - [list](http://sack.sourceforge.net/sack__containers__list.html) - items tracked by dynamic sized array of pointers to userdata
  - [data list](http://sack.sourceforge.net/sack__containers__data_list.html) - Items are tracked by a dynamic sized array of structs
  - [Queue](http://sack.sourceforge.net/sack__containers__queue.html) - tracks a queue of pointers to userdata.
  - [Data QUeue](http://sack.sourceforge.net/sack__containers__data_queue.html) - Tracks a queue with a dynamic array of structures.
  - [Link Stack](http://sack.sourceforge.net/sack__containers__link_stack.html) - stack using a dynamic array of pointers to userdata
  - [Data Stack](http://sack.sourceforge.net/sack__containers__data_stack.html) - Stack using dynamic array of structs.
  - [sets](http://sack.sourceforge.net/sack__containers__sets.html) - A fixed length slab of data structure which are tracked by a bit field of allocated/free members in the set.
  - [Binary tree](http://sack.sourceforge.net/sack__containers__BinaryTree.html) - binary tree using 'set's of nodes that contain pointers to userdata and userkey information.
  - [Text](http://sack.sourceforge.net/sack__containers__text.html) - a type abstraction for tracking strings as linked list of segments... include language text parser for getting phrases and words from other text.
  - Url parsing and building (something like github.com/d3x0r/sack/include/url.h)
- [text](http://sack.sourceforge.net/sack__containers__text.html)
- [Math](http://sack.sourceforge.net/sack__math.html)
  - [Fraction](http://sack.sourceforge.net/sack__math__fraction.html)
  - [Vector](http://sack.sourceforge.net/sack__math__vector.html)
  
