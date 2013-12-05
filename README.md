Comp-Sci
========

Comp Sci 

Takes in a dictionary of words and sorts them into a HashMap.
Each key is the characters in the word rearranged into alphabetical order.
Ex: earth -> aehrt
aehrt is the key

The user now inputs a letters of their choosing and we rearrange the letters as well
rthae -> aehrt

We now search the map for keys that correspond to the rearranged word but we need all
words that contain the letters aehrt not just 'earth'

For this we split our key found from the input rthae -> aehrt and find all possible combinations of the ordered letters
a     e    h    r   t
ae   eh
aeh  ehr
aehr ehrt
aehrt

and so on  but we also have to account for letter skips such as
ahrt
art
at
er
ert
And so we need to find all possible keys.

Once we have the set containing the keys, we compare every key in this set
to those keys read in from the dictionary.
If they match a set from the dictionary is returned containing the list of words able to made.
We add these words to a String.
We continue for every key in our set and finally print our string out.
