#  Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---

##  Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

##  Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

##   Program
```python

if __name__ == '__main__':
    n = int(input())
    records = [[input(), float(input())] for _ in range(n)]
    
    unique_scores = sorted(set(score for _, score in records))
    second_lowest = unique_scores[1]
    
    names = sorted(name for name, score in records if score == second_lowest)
    print(*names, sep='\n')


```

## Output

![image](https://github.com/user-attachments/assets/f6e4cd8f-0028-4d25-b4b9-28d279776e7a)

## Result
Thus, the program has been executed successfully.

