# Shell Scripting (Linux / Bash)

## 1. Foundations

### 1.1 What Is a Shell?

* 1.1.1 Role of the shell in Unix/Linux
* 1.1.2 Shell vs terminal vs console
* 1.1.3 Common shells (sh, bash, zsh, fish)

### 1.2 Command Line Basics

* 1.2.1 Command structure (command, arguments, options)
* 1.2.2 Built-in vs external commands
* 1.2.3 Getting help (`man`, `info`, `--help`)

### 1.3 File System Basics

* 1.3.1 Linux directory hierarchy
* 1.3.2 Absolute vs relative paths
* 1.3.3 Navigation commands

---

## 2. Files, Directories, and Inspection

### 2.1 File and Directory Operations

* 2.1.1 Creating, copying, moving, deleting
* 2.1.2 Recursive operations
* 2.1.3 Globbing and wildcards

### 2.2 File Inspection and Metadata

* 2.2.1 `file` command (file type detection)
* 2.2.2 `stat` (inode and metadata)
* 2.2.3 Timestamps (atime, mtime, ctime)

### 2.3 Permissions and Ownership

* 2.3.1 Permission bits and modes
* 2.3.2 Ownership and groups
* 2.3.3 Special permissions (setuid, setgid, sticky bit)

### 2.4 File Discovery and Analysis (➕)

* 2.4.1 `find` (tests, actions, pruning)
* 2.4.2 `locate` and indexing
* 2.4.3 Disk usage tools (`du`, `df`)

---

## 3. Streams, Redirection, and Text Processing

### 3.1 Standard Streams

* 3.1.1 stdin, stdout, stderr
* 3.1.2 Redirection operators
* 3.1.3 File descriptors

### 3.2 Pipes and Filters

* 3.2.1 Pipe mechanics
* 3.2.2 Command chaining
* 3.2.3 Pipeline error handling

### 3.3 Text Processing Tools

* 3.3.1 `grep` and regex basics
* 3.3.2 `sed` stream editing
* 3.3.3 `awk` field and record processing

### 3.4 Stream Control Utilities

* 3.4.1 `xargs`
* 3.4.2 `tee`
* 3.4.3 `sort`, `uniq`, `cut`, `paste`, `tr`

---

## 4. Environment and Shell Behavior

### 4.1 Variables and Environment

* 4.1.1 Shell vs environment variables
* 4.1.2 Exporting and scoping
* 4.1.3 Common environment variables

### 4.2 Shell Initialization

* 4.2.1 Login vs interactive shells
* 4.2.2 Startup files
* 4.2.3 Environment customization

### 4.3 Command Resolution

* 4.3.1 `$PATH` lookup
* 4.3.2 Aliases and functions
* 4.3.3 Command introspection

### 4.4 Locale and Encoding (➕)

* 4.4.1 `LANG`, `LC_*`
* 4.4.2 Unicode and encoding issues
* 4.4.3 Sorting and collation effects

---

## 5. Writing and Running Scripts

### 5.1 Script Fundamentals

* 5.1.1 Shebang and execution
* 5.1.2 Permissions and portability
* 5.1.3 Script layout

### 5.2 Exit Codes and Status

* 5.2.1 Exit codes
* 5.2.2 `$?` and error propagation
* 5.2.3 Explicit exits

### 5.3 Comments and Style

* 5.3.1 Commenting conventions
* 5.3.2 Readability
* 5.3.3 Script headers and documentation

---

## 6. Variables, Expansion, and Quoting

### 6.1 Variable Basics

* 6.1.1 Assignment and usage
* 6.1.2 Quoting rules
* 6.1.3 Command substitution

### 6.2 Parameter Expansion

* 6.2.1 Defaults and fallbacks
* 6.2.2 String manipulation
* 6.2.3 Length and slicing

### 6.3 Arithmetic Expansion

* 6.3.1 Integer math
* 6.3.2 `(( ))` usage
* 6.3.3 Common pitfalls

### 6.4 Word Splitting and Globbing Internals

* 6.4.1 IFS behavior
* 6.4.2 Quote removal
* 6.4.3 Expansion order

---

## 7. Control Flow

### 7.1 Conditionals

* 7.1.1 `if / elif / else`
* 7.1.2 Test expressions
* 7.1.3 Logical operators

### 7.2 Case Statements

* 7.2.1 Pattern matching
* 7.2.2 Fall-through logic
* 7.2.3 Dispatch patterns

### 7.3 Loops

* 7.3.1 `for`, `while`, `until`
* 7.3.2 Loop control
* 7.3.3 Iteration patterns

---

## 8. Functions and Script Structure

### 8.1 Functions

* 8.1.1 Definition and invocation
* 8.1.2 Parameters and returns
* 8.1.3 Scope and locality

### 8.2 Modular Scripts

* 8.2.1 Sourcing files
* 8.2.2 Shared libraries
* 8.2.3 Configuration separation

### 8.3 Reusability Patterns

* 8.3.1 Utility functions
* 8.3.2 Script APIs
* 8.3.3 Versioning helpers

---

## 9. Input, Arguments, and Options

### 9.1 Positional Parameters

* 9.1.1 `$0`, `$1`, `$@`, `$#`
* 9.1.2 `shift`
* 9.1.3 Argument validation

### 9.2 User Input

* 9.2.1 `read`
* 9.2.2 Defaults and prompts
* 9.2.3 Secure input

### 9.3 Option Parsing

* 9.3.1 Manual parsing
* 9.3.2 `getopts`
* 9.3.3 Usage and help output

---

## 10. Process and Job Control

### 10.1 Processes

* 10.1.1 Foreground/background
* 10.1.2 Process states
* 10.1.3 Signals

### 10.2 Job Control

* 10.2.1 `jobs`, `fg`, `bg`
* 10.2.2 Suspending and resuming
* 10.2.3 Process groups

### 10.3 Traps and Cleanup

* 10.3.1 `trap`
* 10.3.2 Temporary files
* 10.3.3 Graceful termination

### 10.4 Resource Limits and Control

* 10.4.1 `ulimit`
* 10.4.2 Niceness and priority
* 10.4.3 CPU and memory awareness

---

## 11. Error Handling and Debugging

### 11.1 Defensive Bash

* 11.1.1 `set -e`, `-u`, `pipefail`
* 11.1.2 Explicit checks
* 11.1.3 Fail-fast design

### 11.2 Debugging Techniques

* 11.2.1 `set -x`
* 11.2.2 Debug output
* 11.2.3 Reproducible failures

### 11.3 Logging

* 11.3.1 File logging
* 11.3.2 Timestamps and levels
* 11.3.3 Syslog

---

## 12. Advanced Bash Features

### 12.1 Arrays

* 12.1.1 Indexed arrays
* 12.1.2 Associative arrays
* 12.1.3 Iteration and expansion

### 12.2 Advanced Expansions

* 12.2.1 Brace expansion
* 12.2.2 Process substitution
* 12.2.3 Extended globbing

### 12.3 Subshells and Grouping

* 12.3.1 Subshell behavior
* 12.3.2 `{}` vs `()`
* 12.3.3 Performance implications

---

## 13. Networking Fundamentals (Shell-Oriented)

### 13.1 Network Inspection Tools

* 13.1.1 `ip`, `ss`, `ping`
* 13.1.2 `netstat` (legacy)
* 13.1.3 Interface and route inspection

### 13.2 Network Utilities

* 13.2.1 `curl` and `wget`
* 13.2.2 `nc` (netcat)
* 13.2.3 DNS tools (`dig`, `nslookup`)

### 13.3 Networking in Scripts

* 13.3.1 Checking connectivity
* 13.3.2 Downloading and uploading data
* 13.3.3 Timeouts and retries

### 13.4 Remote Access and Transfer

* 13.4.1 `ssh`
* 13.4.2 `scp`, `rsync`
* 13.4.3 Non-interactive authentication

---

## 14. Portability, Performance, and Best Practices

### 14.1 Bash vs POSIX sh

* 14.1.1 Compatibility differences
* 14.1.2 Writing portable scripts
* 14.1.3 Feature detection

### 14.2 Performance

* 14.2.1 Avoiding unnecessary forks
* 14.2.2 Built-ins vs external commands
* 14.2.3 Scaling scripts

### 14.3 Style and Quality

* 14.3.1 Naming and structure
* 14.3.2 Documentation
* 14.3.3 ShellCheck and linting

---

## 15. Real-World Automation

### 15.1 File and System Automation

* 15.1.1 Backups and archiving
* 15.1.2 Monitoring changes
* 15.1.3 Cleanup jobs

### 15.2 System and Network Tasks

* 15.2.1 Service checks
* 15.2.2 Network monitoring
* 15.2.3 Deployment helpers

### 15.3 Scheduling and Integration

* 15.3.1 `cron`
* 15.3.2 Timers (`systemd` timers)
* 15.3.3 CI/CD hooks
