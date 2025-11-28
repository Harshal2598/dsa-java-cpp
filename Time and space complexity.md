Resource for learning Time and Space complexity:
https://www.youtube.com/watch?v=FPu9Uld7W-E
This video explains time complexity and space complexity in the context of coding interviews and problem-solving.

Here's a summary of the key points:

What is Time Complexity? It's not the actual time a program takes to run, as that depends on the machine. Instead, it's the rate at which the time taken increases with respect to the input size (3:46).
Why is it important? Interviewers use it to judge your code's efficiency, not by running it, but by analyzing its theoretical performance (1:16).
Big O Notation: Time complexity is expressed using Big O notation (e.g., O(n), O(n^2), O(log n)) because it provides a standardized way to describe performance independent of hardware (6:11).
Rules for Computing Big O:
Always consider the worst-case scenario (10:40).
Avoid constants because they become insignificant with large inputs (14:05).
Avoid lower values or less significant terms (16:23).
Space Complexity: This refers to the memory space your program takes (26:00). It's calculated as auxiliary space (extra space used to solve the problem) plus input space (space to store the input) (26:50).
Important Rule for Space Complexity: Avoid modifying the input data unless explicitly told to by the interviewer, as it's a bad practice in software engineering (30:26).
Competitive Programming Insight: Most competitive programming servers execute roughly 10^8 operations in one second (32:39), which helps in analyzing if your solution will pass within time limits.
