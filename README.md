# Customised Virtual File System (CVFS)

## 📌 Project Overview

Customised Virtual File System (CVFS) is a system programming project written in C that simulates the core functionality of the Linux File System.
The project provides a Linux-like environment through a custom shell where users can perform file operations such as create, open, read, write, delete, and list files.

## This project helps in understanding :

* File system architecture
* System calls
* Memory management
* OS internal data structures

---

## 🛠 Technology Used

Language: C

Concepts:

* System Programming
* File Handling
* Memory Management
* Data Structures
* Operating System Internals

---

## ✨ Features
- Linux-like custom shell for file operations
- Simulated system calls
- File permission handling


## Custom Shell Interface

Provides a Linux-like environment for performing file operations.

---

## Supported Commands
```
create <filename> <permission>   → Create a new file
open <filename> <mode>           → Open an existing file
read <fd> <size>                 → Read data from file
write <fd>                       → Write data into file
close <fd>                       → Close the file
ls                               → List all files
stat <filename>                  → Display file information
unlink <filename>                → Delete a file
help                             → Display command information
exit                             → Terminate CVFS
```

## System Call Simulation

The following Linux-like operations are implemented using custom functions:

| Linux Operation | Function Name |
| --------------- | ------------- |
| creat()         | CreateFile()  |
| open()          | OpenFile()    |
| read()          | ReadFile()    |
| write()         | WriteFile()   |
| close()         | CloseFile()   |
| unlink()        | UnlinkFile()  |
| stat()          | StatFile()    |

---
## Platform Independent

Runs on any operating system using a C compiler (Windows / Linux / Ubuntu).
---

## 📂 Project Structure
```
CVFS/
│
├── Src/
│   └── cvfs.c      → Main source code
├── Include/        → Header files (if any)
└── README.md
```
---

## ⚙️ Compilation & Execution

Linux / Ubuntu
```
gcc cvfs.c -o Myexe
./Myexe
```

Windows (MinGW)

```
gcc cvfs.c -o Myexe.exe
Myexe.exe
```

## 💻 Example Usage
```
Marvellous CVFS > create Demo.txt 3
File successfully created

Marvellous CVFS > write 3
Enter data:
Jay Ganesh

Marvellous CVFS > read 3 10
Jay Ganesh

Marvellous CVFS > ls
Demo.txt

Marvellous CVFS > unlink Demo.txt
File deleted

Marvellous CVFS > exit
```
---
## 📈 Future Improvements

* Directory support
* Persistent storage (save data to disk)
* Command history
---

## 👨‍💻 Author

CR Dugade 
Aspiring Software Developer

GitHub: https://github.com/crd-codes
LinkedIn: https://linkedin.com/in/chakradhar-dugade
Email : crofficialuse@gmail.com 
