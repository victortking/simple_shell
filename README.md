# Basic Shell (hsh)

A basic shell program written in C language, featuring common shell functionalities. This project was developed by Victor Fredrick.

## Table of Contents

- [Description](#description)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Builtin Commands](#builtin-commands)
- [Shell Operators](#shell-operators)
- [Variables](#variables)
- [Contributing](#contributing)

## Description

This project is a basic shell program written in C language. It allows users to execute commands, handle arguments, and perform various shell operations like handling PATH, environment variables, and built-in commands. The shell also supports logical operators, command separators, and variable replacement. Additionally, it provides functionalities for aliasing and handling comments.

## Features

- Command execution
- Argument handling
- Error handling
- End of file condition with Ctrl + D
- PATH handling
- `exit` builtin command
- `env` builtin command
- `setenv` and `unsetenv` builtin commands
- `cd` builtin command
- Logical operators (&& and ||)
- Command separator (;)
- `alias` builtin command
- Variables replacement
- `$?` variable
- `$$` variable
- Comment support (#)

## Installation

To compile the shell, use the following command:

```
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
```

## Usage

To execute the shell, run the following command:

```
./hsh
```

After running the command above, the shell will start, and you can enter commands as you would in a regular shell.

## Builtin Commands

The shell supports the following builtin commands:

- `exit`: Exits the shell.
- `env`: Prints the current environment.
- `setenv`: Sets an environment variable.
- `unsetenv`: Unsets an environment variable.
- `cd`: Changes the current directory.
- `alias`: Creates or lists aliases.

To use these builtin commands, simply enter the command name followed by any required arguments.

## Shell Operators

The shell supports the following logical operators:

- `&&`: Executes the next command only if the previous command succeeds (returns exit status 0).
- `||`: Executes the next command only if the previous command fails (returns exit status non-zero).

## Variables

The shell supports the following variables:

- `$?`: Contains the exit status of the last executed command.
- `$$`: Contains the process ID of the shell itself.

To use these variables, simply include them in your commands or scripts as needed.

## Contributing

As the sole contributor to this project, I am not currently accepting external contributions. However, if you have any suggestions or feedback, feel free to open an issue on the repository.
