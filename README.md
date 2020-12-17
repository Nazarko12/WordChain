# WordChain

# Description of the laboratory:
Two participants play a linguistic game. At the beginning of the game there is a list of N words. The first player chooses an arbitrary word w1 and deletes one arbitrary letter from it so to get another word w2 from this list. After that the course passes to another player, and he tries to do the same with the word w2.
The game ends in one of two cases:
• There is one word left.
• It is impossible to delete any letter so as to get another word from the dictionary.

Determine the length of the maximum chain that can be achieved in this game given words.

# Problem solving:
First, I used the function to determine the order of each subsequent word in the array by length. In line 8 of his laboratory, a dictionary has been created, which is currently empty. The variable "maximum chain of letters" was also created, which was assigned zero at the beginning.

Used the loop "for" to search for an available word in the dictionary of words. Variable iterator_of_start = 0, because we start the game with the first word in the line. Variable current_max_word = 1, because we started the selection with a random word.

In the "while" cycle:

As long as the variable iterator_of_start < len (available_word), all possible subsequent words formed from the length of the existing word will be written. By going through all the possible options, you can achieve the maximum length of this chain of words. The place where the word should be located depends on its length. This is how a kind of deletion of one letter in a word is formed to create another word in the chain. After all, the word with the most letters will be the first in the list. The last index will correspond to the smallest word.

Line 25 has a function that is designed to read words from a file. This_date = [] is an array of specified letters. The loop assumes the moment when the word is equal to an empty line. Then we leave the cycle and add this word to the end of the list.

Print(largest_string_chain(words)).

# The complexity of the algorithm:

The complexity of my algorithm and this problem is O(n x n). Because I use a loop to go through an array of words, determining the largest word and the relative words from it. The words in the array are not sorted by number of letters. First of all, the task is to determine which of the given words should correspond to this or that place in the array.
Another loop is needed to insert each word in the correct location. Thus, the insertion method is formed. Part of this code refers to quadratic complexity.



# Using:

Programming language: Python.

Firstly, download repository: git clone https://github.com/Nazarko12/WordChain.git. Then you need to open package: "cd WordChain". After this.. Go to the branch "lab4": "git checkout lab4". Run the file: words_chain.py.
