# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```py
with open('story.txt', 'w') as file:
    file.write("This is the first line.\n")
    file.write("Another line begins here.\n")
    file.write("Totally tubular text.\n")
    file.write("hello world.\n")
    file.write("Testing again.\n")
    file.write("Final line.\n")

count = 0
with open('story.txt', 'r') as file:
    for line in file:
        stripped = line.lstrip()
        if stripped and stripped[0] != 'T':
            count += 1

print("Number of lines not starting with 'T':", count)
```

## Output
<img width="802" height="397" alt="image" src="https://github.com/user-attachments/assets/4c7f74ad-96b0-48be-813d-212ffeb9937a" />

## Result
Successfully wrote a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.
