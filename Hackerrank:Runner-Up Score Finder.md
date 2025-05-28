#  Hackerrank:Runner-Up Score Finder in Python

##  AIM:
To write a Python program that takes a list of scores from participants and finds the **runner-up score** (i.e., the second-highest score), eliminating any duplicates.

---

##  ALGORITHM:

1. **Start**
2. Create a variable `n` and get its value from the user (number of participants)
3. Read the list of `n` scores from the user using `input().split()` and convert them to integers
4. Store the scores in a list
5. Use `set()` to remove any duplicate scores
6. Convert the set back to a list and sort it in ascending order
7. Print the second-last element of the sorted list (i.e., the runner-up score)
8. **Stop**

---

##  PROGRAM:
```python

n = int(input())
scores = sorted(set(map(int, input().split())))
print(scores[-2])

```

## OUTPUT

![image](https://github.com/user-attachments/assets/ea4b9484-a2e1-4d67-80cb-abec441e006c)

## RESULT
Thus, the program has been executed successfully.
