# Name #
Associative Array

### Wikipedia Link ###
http://en.wikipedia.org/wiki/Associative_array

## Description ##
An associative array is an abstract data structure that associates keys with
values.

### Data Structure Operations ###

### Implementation in pseudocode ###
There are many different ways of implementing associative arrays though they
are generally implemente using hash tables.

## Use Cases ##
Since associative arrays are usually implemented as a hash table, associative
arrays can be used in any use case a hash table would be used in.  Associative
arrays also have additional benefits over hash tables since they bring in the
benefits of arrays such as being iterable.

## Implementations ##
Associative arrays are typically stored as hash tables with extra space and
logic dedicated to properties such as iteration.  In special use cases,
associative arrays may be implemented using simpler data structures such as a
linked list or normal array.  These data structures may have restrictions on
size or type of key but are easier to implement.

## Related Algorithms And Data Structures ##
### Hash Table ###
Almost all implementations of associative array use hash tables.
### Array ###
Arrays are similar to associative arrays except for the restriction that arrays
are indexed by some integer value which is translated directly into a memory
location rather than being indexed by any value which is hashed before being
translated.
