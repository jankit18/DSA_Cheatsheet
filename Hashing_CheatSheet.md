Hashing:  Finding exact value in a faster way for present or future use.

Direct Address Table Hashing: Simply it uses the array indices to match the value asked and check whether it is hit or not.

Disadvantage: This technique fails for the larger value, floating-point values, string ,and other non-integer values.


Hashing Using Hash Function: We use a hash function that maps the universe of the key with some finite length table using some hash function.
 
Few points to be kept in mind while selecting hash function :
1. It should always map a large Key to some small key.
2. It should generate value from 0 to n-1, where n is the size of the table.
3. It should make the operations like insert, delete and search faster, O(1) for integers and O(size) for a string of length 'size' on an average.
4. It should uniformly distribute the keys into the Hash Table Slots. (MOST IMPORTANT)

Few Hash Functions:
1. Using Modulo Property that modulo with any number M generates a number from 0 to M-1.
   H(large_key) = large_key % M. where M is a prime number greater than hash table size.

2. We use weighted sum for the hash function of string.
   str="abcd"
   H(str) = str[0]*x^0 + str[1]*x^1 + str[2]*x^2 +str[3]*x^3.

3. Universal Hashing - It's a mixture of several hash functions.


@ Since the hashtable size is smaller than the set of universal, the collision of keys will take place.

:) Following are the techniques to tackle collision problems:-

~ If the keys are known in advance we can use a technique called Perfect Hashing. (Wikipedia says:  In computer science, a perfect hash function for a set S is a hash function that maps distinct elements in S to a set of integers, with no collisions).

~ But if we do not know the keys in advance then the following are the techniques which will help us :) 

1. Chaining -> It links the keys with same hash value as chain which can be implemented using a dynamic array or LinkedList or even using self-balancing BST.
	
       Keys = { 21, 58, 17, 54, 50, 102, 8, 159, 205,506, 711, 544, 989 }
       H(key) = key%5

            ------
       0   |  50  | -> 205
	          ------
       1   |  21  | -> 506 -> 711
	          ------
       2   |  17  | -> 102
	           ------
       3   |  58  | -> 8
	          ------
       4   |  54  | -> 159 -> 544 -> 989
	          ------
		
2. Open Addressing -> 
   i. Linear Probing.
  ii. Quadratic Probing.
 iii. Double Hashing.

