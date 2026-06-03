# Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program
```py
list1 = [10, 20, 30, 40]
try:
    value = list1[5]
    print("Accessed value:", value)
except IndexError:
    print("You're out of list range")
```

## Output
<img width="372" height="187" alt="image" src="https://github.com/user-attachments/assets/df3963ec-e161-42bd-832b-24aefe9dcab2" />

## Result
Successfully wrote a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.
