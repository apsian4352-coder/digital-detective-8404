# Mission 2 — Become comfortable with the Terminal

## 1. Task / objective
Learn basic Terminal navigation, practice creating, copying, renaming, and reading files safely, understand flags and pipes, and check out package managers.

## 2. Work completed
- Practiced core Unix commands (`pwd`, `ls`, `cd`, `mkdir`, `touch`, `cp`, `mv`, `cat`).
- Created a `terminal-practice` folder to safely test file overwriting (`>`), appending (`>>`), copying, and renaming.
- Tested `ls -lah` flags and piped output to `head -n 5`.
- Checked my Homebrew package manager setup.

## 3. Commands / tools used
- `pwd`: Prints current directory path.
- `ls`, `ls -l`, `ls -lah`: Lists files with different detail levels.
- `cd` and `cd ..`: Moves between folders.
- `mkdir`: Creates a new folder.
- `touch`: Creates an empty file.
- `cp`: Copies a file.
- `mv`: Renames or moves a file.
- `cat`: Shows file content in terminal.
- `>` and `>>`: Overwrites vs appends text to a file.
- `|` with `head -n 5`: Passes output to show only the top 5 lines.
- `brew --version`: Checked Homebrew version (`Homebrew 7.0.7`).

## 4. My understanding

### Task 2.1 — Terminal Operations Table

| Operation / command name | What it does | What I observed |
| :--- | :--- | :--- |
| Current-directory display (`pwd`) | Shows full path to the current folder. | Printed `/Users/sanjay/project `. |
| Directory listing (`ls`) | Lists files and folders. | Showed my mission folders. |
| Detailed listing (`ls -l`) | Shows permissions, owner, size, and date. | Showed columns with `-rw-r--r--`, `sanjay`, and file size. |
| Change directory (`cd ..` and `cd -`) | Moves to parent or previous directory. | Moved up one level, then right back. |
| Create directory (`mkdir`) | Makes a new folder. | Made `terminal-practice` folder. |
| Create empty file (`touch`) | Creates an empty file. | Created a new 0-byte file without errors. |
| Copy file (`cp`) | Makes a duplicate file. | Made `notes_backup.txt` while keeping the original. |
| Move / rename file (`mv`) | Renames or moves a file. | Renamed backup to `notes_backup_renamed.txt`. |
| Display file contents (`cat`) | Prints file contents in terminal. | Displayed the text lines on screen. |

### Task 2.2 — Safe File Practice Questions
- **Replacing vs adding to the end:** `>` wipes whatever was in the file and starts fresh. `>>` adds new text at the end without touching existing lines.
- **Copying vs moving:** `cp` creates an extra duplicate file so you have two copies. `mv` changes the name or moves it, so only one file remains.
- **What `pwd` tells you:** It gives the exact full path from root `/` to where your terminal currently is, so you know where you are before running commands.
- **Why `ls` is useful:** It lets you see what files exist, verify that a file was created or renamed, and check permissions and sizes.

### Task 2.3 — Flags and Pipes
- **Flags:** `ls` just lists names. With `-l` it gives full details, `-a` includes hidden files (like `.git`), and `-h` makes file sizes easy to read (like KB or MB instead of raw bytes).
- **Pipes:** `ls -la | head -n 5` uses the pipe `|` to take the output of `ls -la` and send it directly into `head -n 5`, which cuts it down to just the first 5 lines.

### Task 2.4 — Package Managers
Homebrew is the package manager on my Mac (`Homebrew 7.0.7`). A package manager is super useful because it lets you install, update, and remove developer tools with a single terminal command instead of manually searching websites and downloading installer files.

## 5. Difficulties faced
At first, I accidentally used a single `>` and overwrote my first line of text.

## 6. How I resolved them
I learned that `>` means overwrite, while `>>` means append. I re-ran with `>>` and both lines stayed in the file.

## 7. Evidence / files
- `mission-02-terminal/README.md`
- `terminal-practice/notes.txt`
- `terminal-practice/notes_backup_renamed.txt`

## 8. Commit details
- Commit message: `Complete Terminal and file management mission`
- Status: Committed to `main`.
