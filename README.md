# Minishell
<div align="center">
  <img src="https://img.shields.io/badge/norminette-passing-success"/>
  <img src="https://img.shields.io/badge/42-project-000000"/>
</div>

## 💡 About
> A minimalist shell implementation that mimics basic bash functionality
This project involves creating a simple shell that handles command execution, pipes, redirections, environment variables, and built-in commands, providing a fundamental understanding of Unix processes and file descriptors.

## 🛠️ Usage
### Requirements
- GNU Make
- GCC
- GNU Readline library
- Unix-like operating system

### Instructions
**1. Compiling**
```shell
$ git clone https://github.com/wdaoudi-/minishell
$ cd minishell
$ make
```
**2. Running the program**
```shell
$ ./minishell
```

## 📋 Features
### Core Features
| Feature | Description |
|---------|-------------|
| Command Execution | Execute commands with absolute/relative paths |
| Built-in Commands | Implementation of: echo, cd, pwd, export, unset, env, exit |
| Signal Handling | Handle ctrl-C, ctrl-D, ctrl-\ |
| Environment Variables | Handle environment variables ($ followed by characters) |
| Input/Output Redirections | Support for <, >, >>, << redirections |
| Pipes | Handle multiple pipe operations |
| Quotes | Support for single and double quotes |

### Built-in Commands
- `echo` with option -n
- `cd` with relative or absolute path
- `pwd` without options
- `export` without options
- `unset` without options
- `env` without options or arguments
- `exit` without options

## ⚙️ Implementation Details
### Architecture
- Command parsing and tokenization
- Environment variable management
- Process creation and management
- File descriptor handling
- Signal handling
- Error management

### Technical Choices
- Written in C
- Follows 42 School's Norm
- Uses readline library for input handling
- Implements memory management to prevent leaks

## 🚨 Error Management
- Command not found handling
- Permission denied cases
- Syntax error detection
- Memory allocation failure handling
- File operation error management

## 🧪 Testing
```shell
$ ./minishell
minishell> ls -la
minishell> echo $PATH
minishell> cat file.txt | grep "pattern" > output.txt
```

## 📚 Resources
- [GNU Bash Reference Manual](https://www.gnu.org/software/bash/manual/bash.html)
- [Unix System Calls](https://man7.org/linux/man-pages/dir_section_2.html)
- [Readline Documentation](https://tiswww.case.edu/php/chet/readline/readline.html)

## 🗣️ About
### Contributing
This project was developed as part of the 42 school curriculum by:
- [wdaoudi-](https://github.com/wdaoudi-)
- [ayarab](https://github.com/ayarab)

---
Made with ❤️ by [wdaoudi-](https://github.com/wdaoudi-) and [ayarab](https://github.com/ayarab)
