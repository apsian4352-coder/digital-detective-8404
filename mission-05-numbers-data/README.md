# Mission 5 — Numbers and data

## 1. Task / objective
Convert numbers between decimal, binary, and hexadecimal by hand, verify them with Python, build a 5-line number converter script, and learn how computers store text with ASCII.

## 2. Work completed
- Did 7 manual number conversions step by step.
- Verified all 7 answers in Python using `bin()`, `hex()`, and `int()`.
- Wrote and tested a 5-line script `number_converter.py`.
- Looked up ASCII codes for 'A' and 'a'.

## 3. Commands / tools used
- Python interactive shell: Checked conversions.
- `python3 mission-05-numbers-data/number_converter.py`: Tested my converter program.
- Built-in functions: `int()`, `bin()`, `hex()`, `ord()`.

## 4. My understanding

### Task 5.1 — Manual Conversions

| Question | Your working and answer |
| :--- | :--- |
| Convert decimal 13 to binary | 13 / 2 = 6 r 1<br>6 / 2 = 3 r 0<br>3 / 2 = 1 r 1<br>1 / 2 = 0 r 1<br>Answer: **1101₂** |
| Convert decimal 25 to binary | 25 / 2 = 12 r 1<br>12 / 2 = 6 r 0<br>6 / 2 = 3 r 0<br>3 / 2 = 1 r 1<br>1 / 2 = 0 r 1<br>Answer: **11001₂** |
| Convert binary 1010 to decimal | (1 × 8) + (0 × 4) + (1 × 2) + (0 × 1) = 8 + 0 + 2 + 0 = **10** |
| Convert binary 1101 to decimal | (1 × 8) + (1 × 4) + (0 × 2) + (1 × 1) = 8 + 4 + 0 + 1 = **13** |
| Convert hexadecimal A to decimal | A in hex is 10 in decimal: (10 × 1) = **10** |
| Convert hexadecimal 1F to decimal | (1 × 16) + (15 × 1) = 16 + 15 = **31** |
| Convert binary 1111 to hexadecimal | 8 + 4 + 2 + 1 = 15 = **F₁₆** (or 0xF) |

### Task 5.2 — Python Verification

| Expression tested | Result | Matches manual calculation? |
| :--- | :--- | :--- |
| `bin(13)` | `'0b1101'` | Yes |
| `bin(25)` | `'0b11001'` | Yes |
| `int('1010', 2)` | `10` | Yes |
| `int('1101', 2)` | `13` | Yes |
| `int('A', 16)` | `10` | Yes |
| `int('1F', 16)` | `31` | Yes |
| `hex(0b1111)` | `'0xf'` | Yes |

### Task 5.3 — Number Converter Program
Here is my 5-line script `number_converter.py`:
```python
num = int(input("Enter a decimal number: "))
b = bin(num)
h = hex(num)
print(f"Binary: {b}")
print(f"Hexadecimal: {h}")
```

**Test results:**

| Test number | Binary output | Hexadecimal output |
| :--- | :--- | :--- |
| 13 | `0b1101` | `0xd` |
| 25 | `0b11001` | `0x19` |
| 42 | `0b101010` | `0x2a` |

`bin()` converts an integer into binary with a `0b` prefix. `hex()` converts an integer into hexadecimal with a `0x` prefix.

### Task 5.4 — How Text Is Stored
- Uppercase `A`: ASCII code `65`.
- Lowercase `a`: ASCII code `97`.
- **Why computers need encoding:** Computers only understand binary numbers (0s and 1s), so they need an agreed code table like ASCII or UTF-8 to know which number stands for which letter.
- **Character outside basic ASCII:** The Rupee symbol `₹` or an emoji like `😊`. Basic ASCII only has 128 characters, so UTF-8 is used for modern symbols.

## 5. Difficulties faced
I wondered why Python outputs `0b` and `0x` in front of the numbers.

## 6. How I resolved them
I learned that `0b` simply means binary and `0x` means hex so programmers know which base the number is in.

## 7. Evidence / files
- `mission-05-numbers-data/number_converter.py`
- `mission-05-numbers-data/README.md`

## 8. Commit details
- Commit message: `Build number converter and practise data representation`
- Status: Committed to `main`.
