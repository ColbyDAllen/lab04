# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

-- We learned how to turn a truth table into a KMAP and pull the minimal cost POS and SOP from said KMAP. Then we learned through the waveforms in Vivado that we could 
confirm whether or not our maxterm and minterm expressions were correct.  

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
-- KMAPS are arranged so that the values wrap around the edges. The squares on opposite sides of the KMAP are adjacent. 
This makes it so that the columns and rows are logically next to each other. 

### Why are the names Sum of Products and Products of Sums?
-- SOPs involve minterms (1's from Truth Table) and POSs involve Maxterms (0's from Truth Table). Respectively, their operational formats are `+(_*_)+` and `*(_+_)*`.

### Open the test.v file – how are we able to check that the signals match using XOR?
-- In test.v XOR is used to compare two signals. For example, the expected output and what is the actual output. If the two signals match, XOR produces 
a 0 (Inputs are the same), and if they're different XOR produces a 1 (Inputs are different). XOR is a way to check they're equal. 

