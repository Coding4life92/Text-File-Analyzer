# Text File Analyzer

A small but powerful command-line tool written in C that analyzes text files and reports useful statistics—such as:

- Total characters  
- Total words  
- Total lines  
- Character frequency  
- Word frequency  

It’s designed to be simple, fast, and easy to extend. The project uses a custom hash table for efficient word counting and a modular analyzer engine.

---

## Features

- Count total characters, words, and lines  
- Show character frequency (printable ASCII only)  
- Show word frequency using a hash table  
- Output results to the terminal **or** a file  
- Clear, flexible command-line options  
- Clean Makefile with rebuild + cleanup targets  

---

## How to Build and Run

### 1. Build the Program

From the project root directory, run:

```sh
make
```

This compiles all .c files and produces the executable:

```sh
./analyzer
```

### 2. Run the Analyzer

```sh
./analyzer [options] <filename>
```

### Command-Line Options
| Option           | Description                                        |
| ---------------- | -------------------------------------------------- |
| `-c`, `-w`, `-l` | Show overall statistics (characters, words, lines) |
| `--freq`         | Show character and word frequency tables           |
| `-o <file>`      | Write the report to a file instead of printing it  |


### Wrtie report to file
```sh
./analyzer -o report.txt edge_cases.txt
```

### Useful Make Commands

Build the program
```sh
make
```

Clean compiled files
```sh
make clean
```

Rebuild from sratch
```sh
make re
```