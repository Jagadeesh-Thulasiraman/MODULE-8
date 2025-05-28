# #  Hackerrank:#  Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

##  Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

##  Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---

##  PROGRAM:
```python

marks = eval(input())

# Calculate total marks
totals = {name: sum(scores) for name, scores in marks.items()}

# Print total marks
print(totals)

# Find topper
top_score = max(totals.values())
for name, total in totals.items():
    if total == top_score:
        print(f"Topper is: {name} with marks = {total}")

```

## OUTPUT

![image](https://github.com/user-attachments/assets/e5100b36-d12b-4df3-95fd-567791da2f1e)

## RESULT
Thus, the program has been executed successfully.
