# Syndicate-Distributions
Syndicate Balancing Algorithm
Overview
The Syndicate Balancing Algorithm is a Python-based solution designed to distribute students into k groups while maintaining an equitable distribution of students, professions, and average scores. This algorithm addresses the challenge of creating balanced groups based on three key criteria:

Equal Group Sizes: Each group should contain a similar number of students. When the total number of students cannot be evenly divided by k, groups may differ by at most one student.

Profession Distribution: Professions among students should be as evenly distributed as possible across all groups. If the total number of students with a specific profession exceeds the number of groups, the algorithm will allow slight variations in distribution.

Minimized Standard Deviation of Average Scores: The algorithm aims to minimize the standard deviation of average scores across the groups, ensuring that group performance is closely aligned.

Features
CSV Data Handling: Loads student data from a CSV file into a Pandas DataFrame.
Sorting Mechanism: Students are sorted based on profession and score to facilitate fair distribution.
Round-Robin Distribution: Implements a round-robin method for distributing students into groups by profession.
Standard Deviation Calculation: Computes the standard deviation of group averages to evaluate the effectiveness of the distribution.
Adaptive Swapping Strategy: Employs a swapping mechanism to iteratively improve group balance by exchanging students between groups based on scores and professions.
Usage
Input Data: Prepare a CSV file with student records, including userId, score, and profession.
Set Group Count: Define the number of groups (k) based on the total number of students.
Run the Algorithm: Execute the script to observe the initial and updated group distributions and their corresponding average scores and standard deviation.
Example
The algorithm has been tested with various datasets, demonstrating its ability to create well-balanced groups that adhere to the outlined criteria.

Requirements
Python 3.x
Pandas
NumPy
