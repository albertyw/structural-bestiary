# Name #
Hash Table

### Wikipedia Link ###
http://en.wikipedia.org/wiki/Hash_table

## Description ##
The hash table data structure is a way of linking variables (keys) to other
variables (values).  Therefore, it is an implementation of an associative
array.  The major benefit of hash tables is that it has constant time insert,
lookup, and deletion, the three of which together beat most other data
structures.

### Data Structure Operations ###
Inserting, reading, updating, and deleting data in a hash table given a key
are all constant time.  For each operation, the key is run through a hashing
function which gives a value that can be easily translated into a memory
address.  Once the address is known, the data at the memory location can be
read or modified.

Given the pigeonhole principle, hash functions may hash different keys to the
same value (i.e. a hash collision).  Hash tables can accommodate collisions in
different ways, usually through some form of a list of data.  This means that
althought the average time for operations is constant, the worst case time for
operations is linear with respect to the number of objects stored in the hash
data structure.

### Implementation in pseudocode ###
Generally, a
hash table has some space allocated in memory with the space covering possible
hash function outputs.  The values in that space are pointers to linked lists
of the values of the hash table.

## Use Cases ##
Hash tables have extremely low time and space costs for all major operations.
Therefore, it is extremely useful for storing any kind of data that has
key/value indexing.  The hash table is also the basis for many other data
structures.

## Implementations ##
Hash tables are implemented natively in almost all programming languages.

## Related Algorithms And Data Structures ##
### Hash Functions ###
Hash tables are heavily based upon the hash functions that are used to compute
their keys.  Hash functions are discussed at http://en.wikipedia.org/wiki/Hash_function

Good hash functions have as low probability of a hash collision as possible.
