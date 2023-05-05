Download Link: https://assignmentchef.com/product/solved-ds-mini-assignment3-hashtable
<br>
Create a program that stores words in a Hash Table and then searches for the words.

<strong>Requirements</strong>

You will keep track of words that are 20 or fewer characters long.  The nodes that you will create as structs will contain an array of char of length 21 and a pointer to the next node.  Call this struct WordNode.

In main, declare an array variable to contain your hash table.  Let the array buckets contain pointers to WordNodes.  The size of the array is 11.

Create a loop that gets one word at a time from the user until they enter “.” as the only thing on the input line.

Each time you get a word, pass the word as a parameter to a hash function.  This hash function must call the djb2 function (from the hash tables lecture; change the parameter to work with chars rather than unsigned chars) and then use the Division Method to return a value between 0 and 10 (inclusive) as a hash value.  Use this returned hash value to determine which bucket should contain the word.  Then add the word to the bucket as described in lecture. Make sure that your linked lists are sorted linked lists, sorted in ascending order (e.g. “alpha” would occur before “theta”).  They do not have to have a tail or prev pointers but they can if you want (the tail pointer would now have to be in the bucket along with the head pointer).

Once the user is done entering words, set up a separate loop to get input for words to search for.  Then search for the words in the hash table by determining the appropriate bucket and searching the linked list found there (if there is one).  Every time you do a comparison in your search, use printf() (or cout) to display the word you are comparing your search word against.  When you find the word, use printf() (or cout) to display “Success!”.  If you don’t find the word, use printf() (or cout) to display “Not there!”.  This will continue in a loop until the user enters “.” as the only thing on the input line.

You should comment as normal.