# Activities

> The [modulo-calculator](#links) might be handy in these exercises.

## Task 1

- Refer to the following link. Discuss how open hashing works.
  https://www.cs.usfca.edu/~galles/visualization/OpenHash.html
  # A:Open hashing takes integer, counts selected modulo and inserts to hash value modulo calculation gives. Example in this link uses modulo 13.  (x modulo 13)
- Open Hashing Practice. Refer to the following link. Move each record on the left to the appropriate bin on the right.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Hashing/OpenHashPRO.html
- Given the following input (`4322, 1334, 1471, 9679, 1989, 6171, 6173, 4199`) and the hash function `x mod 10`, which of the following statements are true?
- [X] `9679, 1989, 4199` hash to the same value
- [X] `1471, 6171` hash to the same value
- [] All elements hash to the same value
- [] Each element hashes to a different value


## Task 2

- Bucket Hashing Practice. Refer to the following [link](https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Hashing/HashBucketPRO.html).
- The keys `12, 18, 13, 2, 3, 23, 5 and 15` are inserted into an initially empty hash table of length `10` using open addressing with hash function `h(k) = k mod 10` and **linear probing**. What is the resultant hash table?
        12  13  2   3   23  5   18   15

0   1   2   3   4   5   6   7    8    9

    12 is index 2
    18 is index 8
    13 is index 3
    2 is index 4
    3 is index 5
    23 is index 6
    5 is index 7
    15 is index 9

## Task 3:

- What is the [Birthday Paradox](http://en.wikipedia.org/wiki/Birthday_problem)?
# A: Because of the probability of collision
- Why is it generally discussed with hashing?
# A: Ratkaistaan törmäysongelmia hashingilla
- In a hash table of 9658 slots, what is the smallest number of records that must be inserted for the probability of a collision to be 61% or more? Use the calculator at this [link](https://opendsa-server.cs.vt.edu/ODSA/AV/Hashing/Birthday.html)
# A: 136
- Discuss in groups how the following program works `./src/birthday.cpp`?

## Task 4: Individual (at home)

- Difference between `Separate Chaining` and `Open Addressing` collision handling techniques?

  https://www.geeksforgeeks.org/open-addressing-collision-handling-technique-in-hashing/

  # A: All items are stored directly in the hash table, and collisions are resolved by finding an empty slot using a predefined sequence of probe locations. This means that if a slot is already occupied, the algorithm will probe the next slot until an empty slot is found. There are several methods for generating probe sequences, such as linear probing, quadratic probing, and double hashing.

  https://www.geeksforgeeks.org/separate-chaining-collision-handling-technique-in-hashing/

  # A: In this technique, each hash table slot is a linked list, and collisions are resolved by adding the new item to the appropriate list. This means that multiple items with different keys can occupy the same slot in the hash table, but they will be stored in different locations in the linked list.

- (Bonus) Run the following program and comment on the code `./src/hashtable.cpp`

# A: The Program is already well commented and I only could add a few comments. The program defines a HashMapTable class that contains methods to insert and delete keys, as well as to display the entire hash table. In the main function, an instance of the HashMapTable class is created with a table size of 6, and the keys {20, 34, 56, 54, 76, 87} are inserted into the hash table using the insertElement method. The key 34 is then deleted using the deleteElement method, and the final state of the hash table is displayed using the displayHashTable method. The output of the program is following:
0 ==> 54
1
2 ==> 20 ==> 56
3 ==> 87
4 ==> 76
5
 


## Link(s)

- [modulo-calculator](https://www.calculators.org/math/modulo.php)
- [Practice Problems on Hashing](https://www.geeksforgeeks.org/practice-problems-on-hashing/)
