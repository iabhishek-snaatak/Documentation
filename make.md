# SOP: Make Build Tool - Installation

## Author Information

| Created by      | Created on         | Version          | Last updated On   | pre Reviewer       | L0 Reviewer     | L1 Reviewer        | L2 Reviewer       |
|-----------------|--------------------|------------------|-------------------|--------------------|-----------------|--------------------|-------------------|
| Abhishek Saini  | 21-07-2025         | V 1.0            | 21-07-2025        | Prashant           | -        | -   | -  |

---

##  Table of Contents
- [Objective](#objective)
- [Prerequisites](#prerequisites)  
- [Step-by-Step Installation Guide](#step-by-step-installation-guide)    
- [Verify & Version Check](#verify--version-check)  
- [Functional Test (Simple Makefile Example)](#functional-test-simple-makefile-example)  
- [Notes](#notes)  
- [Contact Information](#contact-information)  
- [References](#references)  



## Objective

This SOP provides a standardized method to install and validate the GNU Make tool on Ubuntu-based systems. It ensures that `make` is correctly set up for use

---

## Prerequisites

- Operating System: Ubuntu/Debian-based Linux
- User must have `sudo` privileges

---

## Step-by-Step Installation Guide

###  Step 1: Update System Packages

```bash
sudo apt update
```

### 🔹 Step 2: Install Make (and essential build tools)

```bash
sudo apt install build-essential -y
```

*Note:* `build-essential` includes `make`, `gcc`, and other compilation tools.

---

## verify & version check

After installation, validate that `make` is correctly installed and functional:

| Checkpoint                      | Command                           | Expected Output                                    |
|---------------------------------|-----------------------------------|----------------------------------------------------|
| Verify make version             | `make --version`                  | Displays installed make version (e.g. GNU Make 4.x)|
| Check make binary location      | `which make`                      | Should return `/usr/bin/make`                     |

---

## Functional Test (Simple Makefile Example)

### Create test files:

#### 🔸 hello.c

```c
#include <stdio.h>
int main() {
    printf("Hello, Make!\n");
    return 0;
}
```

#### 🔸 Makefile

```makefile
all:
	gcc -o hello hello.c
```

### Run make:

```bash
make
```

### Run the output:

```bash
./hello
```
---

## Notes

- `make` does not compile code by itself; it automates the compilation by reading instructions from a `Makefile`.
- Useful in C/C++ projects and even in DevOps automation pipelines.

- --

## Contact Information

| **Name**           | **Email address**                         |
|--------------------|--------------------------------------------|
| Abhishek saini    | abhishek.saini.snaatak@mygurukulam.co |

---

## References

| **Link**                                                                 | **Description**                                   |
|--------------------------------------------------------------------------|---------------------------------------------------|
| [Make installation guide ](https://www.tutorialspoint.com/makefile/index.htm) | Document format followed from this link.          |
