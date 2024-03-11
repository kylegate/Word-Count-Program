# Word Count Program (C++ with STL)

## Overview

In this sophisticated C++ project, I developed a powerful program to conduct in-depth statistical analysis of word, number, and character usage within a given text file. The project showcases advanced algorithms, efficient data structures, and a meticulous approach to processing textual data.

## Key Features

1. **STL Containers and Algorithms:** Leveraging C++ STL containers and algorithms for dynamic and scalable data management.

2. **Word, Number, and Character Analysis:** Distinguishing between words and numbers based on consecutive sequences of letters or digits, and tracking various character occurrences.

3. **Case-Insensitive Word Counting:** Treating words case-insensitively for enhanced accuracy and flexibility.

4. **Top Ten Ranking:** Identifying and ranking the ten most frequently occurring characters, numbers, and words. Handling tie-breaking situations intelligently.

5. **Analysis.txt Documentation:** Detailed analysis.txt document covering the complexity analysis of critical algorithms and procedures.

6. **Executable Code Verification:** Benchmark executable code adhering to specified formatting standards.

7. **Makefile Implementation:** Comprehensive makefile (proj6.x) for streamlined compilation, resulting in an executable named proj6.x.

8. **Performance Optimization:** Strategic selection of C++ string class and STL containers for optimal "Big-O" complexity.

## Analysis 

Reading the input set
Complexity is O(N): All operations operate on the data size N with dominant linear complexity over constant time.

Storing the characters / words / numbers in your chosen containers, and setting
their tracking values
the worst case Complexity is O(N) because I used an unordered map

Looking up the final tracking info on your character / word / number frequencies
The STL alogirthm sort function is the dominate term in the complexity of the final tracking as it is O(N*Log(N))\

Deciding on (and accessing for output) your "Top Ten" most frequent list for each case
the vector where the top 10 are stored has a O(1) constant time access as the members are indexed.

Any other important algorithm/tasks you perform to complete the job
compare and compare_char both have O(N) time as the structure must be iterated through 
The remaning functions IsWord, IsNumber, and Make_Lowercase are all O(N) because they index through a string
