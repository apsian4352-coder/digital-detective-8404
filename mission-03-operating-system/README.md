# Mission 3 — Understand the operating system

## 1. Task / objective
Explore how the operating system manages hardware, check system information and storage, understand processes and PIDs, and learn about file paths and permissions.

## 2. Work completed
- Checked OS details, my user account, and available disk space.
- Looked at running processes, process IDs (PIDs), and parent PIDs.
- Tested absolute vs relative paths inside the repository.
- Examined file permissions (`r`, `w`, `x`) on a test file.
- Filled out the OS responsibilities table with everyday examples.

## 3. Commands / tools used
- `uname -srm`: Checked the kernel name, version, and architecture (`Darwin 27.2.0 arm64`).
- `whoami` and `id`: Showed user `sanjay` (UID 501, group staff).
- `df -h /`: Showed 371GiB available out of 460GiB.
- Python `os.getpid()` / `os.getppid()`: Looked up active process and parent process IDs.
- `ls -l`: Checked file permissions.

## 4. My understanding

### Task 3.1 — System Details

| Information explored | What it tells you | Your observation (privacy-safe) |
| :--- | :--- | :--- |
| Operating system / system details | Kernel name, version, and CPU architecture. | Darwin 27.2.0 arm64 (macOS on Apple Silicon). |
| Current account identity | Logged-in user account and user ID. | User: sanjay, UID: 501, Group: staff. |
| Available and used storage | Total, used, and free disk space. | APFS drive: 460GiB total, 13GiB used, 371GiB free. |
| System activity snapshot | Active process information. | Current terminal process running under PID 22088 (parent PPID 21894). |

### Task 3.2 — Processes
- **What is a process?** A program that is actively running in memory right now.
- **What is a PID?** Process ID — a unique number the OS gives to every running program so it can track it.
- **Two examples of running processes:** `zsh` (my terminal shell) and `python3` (when I run a Python script).

### Task 3.3 — Paths and Permissions
- **Absolute vs Relative Paths:**
  - Absolute path: The full path starting all the way from root `/`. Example: `/Users/sanjay/project/README.md`.
  - Relative path: The path from wherever you currently are. Example: `mission-03-operating-system/README.md`.
- **Permissions:**
  Checking `notes.txt` showed `-rw-r--r--`:
  - Owner (`sanjay`): `rw-` (can read and write).
  - Group (`staff`): `r--` (can only read).
  - Others: `r--` (can only read).
  - `r` = read, `w` = write, `x` = execute (run as a program or enter a folder).

### Task 3.4 — Operating System Responsibilities

| OS responsibility | Your explanation | Example |
| :--- | :--- | :--- |
| Process management | Decides which program gets CPU time and when. | Letting me listen to music while typing in VS Code. |
| Memory management | Gives RAM to apps and frees it when closed. | Allocating memory to Chrome tabs without crashing other apps. |
| Device management | Talks to hardware using device drivers. | Sending print jobs to a printer via USB or Wi-Fi. |
| File management | Organizes files and folders on the storage drive. | Saving and finding files in APFS folders. |
| User interface / shell | Gives a way for humans to interact with the computer. | macOS desktop interface and the Zsh terminal. |
| Security and permissions | Stops unauthorized users or apps from touching system files. | Asking for my password before changing system settings. |

## 5. Difficulties faced
When I tried running `ps` in my terminal sandbox, it warned about restricted permissions.

## 6. How I resolved them
I used Python's built-in `os.getpid()` and `os.getppid()` to check process IDs safely without needing special permissions.

## 7. Evidence / files
- `mission-03-operating-system/README.md`

## 8. Commit details
- Commit message: `Document operating system and file management`
- Status: Committed to `main`.
