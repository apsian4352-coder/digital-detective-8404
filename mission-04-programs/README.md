# Mission 4 — How programs run

## 1. Task / objective
Create and run a one-line Python program, and compare how compilers and interpreters run code.

## 2. Work completed
- Created `mission-04-programs/hello.py` with 1 line of code.
- Ran it using Python 3 and confirmed the output.
- Made a comparison table between compilers and interpreters.

## 3. Commands / tools used
- Text Editor: Wrote `hello.py`.
- `python3 mission-04-programs/hello.py`: Ran the script.
- Git: Tracked the files.

## 4. My understanding

### Task 4.1 — Python Program
I wrote `hello.py` with one simple line:
```python
print("Hello from Python")
```
I ran `python3 mission-04-programs/hello.py` and it printed:
```text
Hello from Python
```

### Task 4.2 — Compiler vs Interpreter

| Point | Compiler | Interpreter |
| :--- | :--- | :--- |
| When translation happens | Translates the whole file into machine code before running. | Translates and executes line by line at runtime. |
| Typical output | A standalone binary file (like `.exe`). | Runs directly; no separate binary file created. |
| One example | C or C++ (using `gcc` or `clang`). | Python (using `python3`) or JavaScript. |
| One advantage | Very fast execution speed. | Quick testing and easy to run across different computers. |

**Summary:** A compiler translates the whole program all at once into machine code before you run it, creating a separate executable file. An interpreter reads and executes the code line by line while the program is running. Compilers give faster speed, while interpreters make it easier and faster to test changes while coding.

## 5. Difficulties faced
No major difficulties. The script worked on the first try.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-04-programs/hello.py`
- `mission-04-programs/README.md`

## 8. Commit details
- Commit message: `Compare compilers and interpreters`
- Status: Committed to `main`.
