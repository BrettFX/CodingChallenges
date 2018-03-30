## Challenge:
Transform one word into another with four operations: add a letter, delete a letter, change a letter, and take an anagram of the existing word.

### Rules:
- Every interim step between the first and the last word must also be a word
- No interim step can be less than three letters
- The fist line of input will contain the "cost" of each operation in the order above
- The second line of input will contain the starting word.
- The third line of input will contain the ending word.

### Goal:
Find the lowest possible "cost" of transforming the starting word into the ending word. You can use any word list you like -- feel free to include your word list or a link to it as part of your solution. (Depending on your word list, your answer might not be exactly the same as the ones below.)

The solution should detect and handle invalid input, and return -1 if there is no solution.

### Input/Output:
It should suffice to invoke the program with the following command-line arguments:
`insertion_cost deletion_cost replacement_cost anagram_cost starting_word ending_word`

The output should be similar to the following:
`(Output: total_cost) (initial_word_state, word_state_2, word_state_3, ... , word_state_n)`

It is possible to find a solution in one step through the use of an anagram. However, take heed as the cost may not be optimal.

### Example Input/Output:
1 3 1 5 HEALTH HANDS
(Output: 7) (HEALTH, HEATH, HEATS, HENTS, HENDS, HANDS)