# Prajwal's Custom Virtual File System (CVFS)

## 📌 Overview
**Prajwal's Custom Virtual File System (CVFS)** is a system-level project built from scratch using C and C++. It simulates the core internal architecture, memory management, and command-line interface of a Linux-based Operating System. 

Instead of interacting with the physical hard drive, this project creates a virtual file system entirely within the system's Primary Memory (RAM). It manages virtual files using custom-built low-level data structures.

## 🚀 Core Features & Concepts
* **Dynamic Memory Allocation:** Handles memory efficiently to store files and data structures at runtime.
* **Custom Data Structures:** Extensive use of Singly and Doubly Linked Lists to manage the **Inode Table**, **File Table**, and **User File Descriptor Table (UFDT)**.
* **OS Fundamentals Implemented:**
  * **Super Block & Boot Block:** Initializes and manages the total and free inodes.
  * **Inodes (Index Nodes):** Stores metadata for every created file (size, type, permissions, reference count).
  * **File Descriptors:** Maps user requests to the actual file in memory.
* **Interactive Shell:** A custom, infinite-listening command-line interface that executes standard Linux file-handling commands.

## 🛠️ Supported Commands
The CVFS interactive shell supports the following custom commands:

| Command | Usage | Description |
| :--- | :--- | :--- |
| `help` | `help` | Displays the help manual for all commands. |
| `man` | `man [command]` | Displays the manual page for a specific command. |
| `clear` | `clear` | Clears the terminal screen. |
| `ls` | `ls` | Lists all created files and their current sizes. |
| `creat` | `creat [filename] [permission]` | Creates a new file. *(Permissions: 1=Read, 2=Write, 3=Both)* |
| `write` | `write [fd]` | Prompts to write string data into the specified file descriptor. |
| `read` | `read [fd] [bytes]` | Reads a specific number of bytes from a file. |
| `stat` | `stat [filename]` | Displays statistical information and metadata about a file. |
| `unlink` | `unlink [filename]` | Deletes a file and safely frees its allocated memory and inodes. |
| `exit` | `exit` | Safely deallocates all resources and terminates the file system. |

## 💻 How to Compile and Run

### Prerequisites
* A C/C++ compiler (like GCC or MinGW) installed on your system.

### Steps to Execute
1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/pansareprajwal/Custom-Virtual-File-System.git](https://github.com/pansareprajwal/Custom-Virtual-File-System.git)


### 👨‍💻 Author
Prajwal Sanjay Pansare

GitHub: [@pansareprajwal](https://github.com/pansareprajwal)

LinkedIn: [Prajwal Pansare](https://www.linkedin.com/in/prajwalpansare/)
