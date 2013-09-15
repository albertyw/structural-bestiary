# Array #

### Wikipedia Link ###
http://en.wikipedia.org/wiki/Array_data_structure

## Description ##
An Array is a very simple data structure where individual data values are
stored sequentially.  Each value in an Array is associated with an index
which refers to the position of that value relative to other values in the
Array.  Additionally, each value takes the same amount of memory, allowing
the memory locations of values to be easily calculated from the beginning of
the array data structure.

### Data Structure Operations ###
**Insertion**
Inserting a value at an index is linear `O(n)` time with respect to the number
of values already in the array.  This is because inserting a value at an index
requires the rest of the values in the array to be pushed back by one index.

**Reading**
Reading a value given an index is constant `O(1)` time.  The location of the beginning
of the value will be at `(beginning of array) + (index) * (size of value)`

**Deletion/Updating**
Deleting or updating values from an array involves overwriting the value at the
given index with a new value (update) or with a null value (delete).  After
finding the location within the array, deleting or updating the location is
constant time.

### Implementation in pseudocode ###
```
class Array:
    function initialize():
        set ElementSize to be the memory size of each element
        set StartLocation to be the beginning of the memory location of the array

    function memoryLocation(index):
        return StartLocation + index * ElementSize

    function read(index):
        return memoryLocation(index) to memoryLocation(index+1)

    function update(index, element):
        copy element to NewElementLocation
```

## Use Cases ##
The array data structure is one of the best ways to store data that is read or
added sequentially.  When non-sequential access is required, linked lists or
other data structures may be more useful.  Arrays are also extremely simple to
implement and most programming languages natively support array data types.

## Implementations ##
Most languages have a native implementation of array data types already.  (Some
default to linked lists).


## Related Algorithms And Data Structures ##
### Linked Lists ###
Linked Lists are a similar data structure to arrays but they support
non-contiguous values with the trade off that reading arbitrary values is
slower.
### Multidimensional Array ###
Multidimensional arrays are basically the same as normal single dimensional
arrays, except for additional indexes/dimensions which are converted into a
single linear array.
