# Shell Scripting (Linux / Bash)

1. Foundations
    1. What Is a Shell?
        - Role of the shell in Unix/Linux
        - Shell vs terminal vs console
        - Common shells (sh, bash, zsh, fish)
    1. Command Line Basics
        - Command structure (command, arguments, options)
        - Built-in vs external commands
        - Getting help (`man`, `info`, `--help`)
    1. File System Basics
        - Linux directory hierarchy
        - Absolute vs relative paths
        - Navigation commands
1. Files, Directories, and Inspection
    1. File and Directory Operations
        - Creating, copying, moving, deleting
        - Recursive operations
        - Globbing and wildcards
    1. File Inspection and Metadata
        - `file` command (file type detection)
        - `stat` (inode and metadata)
        - Timestamps (atime, mtime, ctime)
    1. Permissions and Ownership
        - Permission bits and modes
        - Ownership and groups
        - Special permissions (setuid, setgid, sticky bit)
    1. File Discovery and Analysis (➕)
        - `find` (tests, actions, pruning)
        - `locate` and indexing
        - Disk usage tools (`du`, `df`)
1. Streams, Redirection, and Text Processing
    1. Standard Streams
        - stdin, stdout, stderr
        - Redirection operators
        - File descriptors
    1. Pipes and Filters
        - Pipe mechanics
        - Command chaining
        - Pipeline error handling
    1. Text Processing Tools
        - `grep` and regex basics
        - `sed` stream editing
        - `awk` field and record processing
    1. Stream Control Utilities
        - `xargs`
        - `tee`
        - `sort`, `uniq`, `cut`, `paste`, `tr`
1. Environment and Shell Behavior
    1. Variables and Environment
        - Shell vs environment variables
        - Exporting and scoping
        - Common environment variables
    1. Shell Initialization
        - Login vs interactive shells
        - Startup files
        - Environment customization
    1. Command Resolution
        - `$PATH` lookup
        - Aliases and functions
        - Command introspection
    1. Locale and Encoding (➕)
        - `LANG`, `LC_*`
        - Unicode and encoding issues
        - Sorting and collation effects
1. Writing and Running Scripts
    1. Script Fundamentals
        - Shebang and execution
        - Permissions and portability
        - Script layout
    1. Exit Codes and Status
        - Exit codes
        - `$?` and error propagation
        - Explicit exits
    1. Comments and Style
        - Commenting conventions
        - Readability
        - Script headers and documentation
1. Variables, Expansion, and Quoting
    1. Variable Basics
        - Assignment and usage
        - Quoting rules
        - Command substitution
    1. Parameter Expansion
        - Defaults and fallbacks
        - String manipulation
        - Length and slicing
    1. Arithmetic Expansion
        - Integer math
        - `(( ))` usage
        - Common pitfalls
    1. Word Splitting and Globbing Internals
        - IFS behavior
        - Quote removal
        - Expansion order
1. Control Flow
    1. Conditionals
        - `if / elif / else`
        - Test expressions
        - Logical operators
    1. Case Statements
        - Pattern matching
        - Fall-through logic
        - Dispatch patterns
    1. Loops
        - `for`, `while`, `until`
        - Loop control
        - Iteration patterns
1. Functions and Script Structure
    1. Functions
        - Definition and invocation
        - Parameters and returns
        - Scope and locality
    1. Modular Scripts
        - Sourcing files
        - Shared libraries
        - Configuration separation
    1. Reusability Patterns
        - Utility functions
        - Script APIs
        - Versioning helpers
1. Input, Arguments, and Options
    1. Positional Parameters
        - `$0`, `$1`, `$@`, `$#`
        - `shift`
        - Argument validation
    1. User Input
        - `read`
        - Defaults and prompts
        - Secure input
    1. Option Parsing
        - Manual parsing
        - `getopts`
        - Usage and help output
1. Process and Job Control
    1. Processes
        - Foreground/background
        - Process states
        - Signals
    1. Job Control
        - `jobs`, `fg`, `bg`
        - Suspending and resuming
        - Process groups
    1. Traps and Cleanup
        - `trap`
        - Temporary files
        - Graceful termination
    1. Resource Limits and Control
        - `ulimit`
        - Niceness and priority
        - CPU and memory awareness
1. Error Handling and Debugging
    1. Defensive Bash
        - `set -e`, `-u`, `pipefail`
        - Explicit checks
        - Fail-fast design
    1. Debugging Techniques
        - `set -x`
        - Debug output
        - Reproducible failures
    1. Logging
        - File logging
        - Timestamps and levels
        - Syslog
1. Advanced Bash Features
    1. Arrays
        - Indexed arrays
        - Associative arrays
        - Iteration and expansion
    1. Advanced Expansions
        - Brace expansion
        - Process substitution
        - Extended globbing
    1. Subshells and Grouping
        - Subshell behavior
        - `{}` vs `()`
        - Performance implications
1. Networking Fundamentals (Shell-Oriented)
    1. Network Inspection Tools
        - `ip`, `ss`, `ping`
        - `netstat` (legacy)
        - Interface and route inspection
    1. Network Utilities
        - `curl` and `wget`
        - `nc` (netcat)
        - DNS tools (`dig`, `nslookup`)
    1. Networking in Scripts
        - Checking connectivity
        - Downloading and uploading data
        - Timeouts and retries
    1. Remote Access and Transfer
        - `ssh`
        - `scp`, `rsync`
        - Non-interactive authentication
1. Portability, Performance, and Best Practices
    1. Bash vs POSIX sh
        - Compatibility differences
        - Writing portable scripts
        - Feature detection
    1. Performance
        - Avoiding unnecessary forks
        - Built-ins vs external commands
        - Scaling scripts
    1. Style and Quality
        - Naming and structure
        - Documentation
        - ShellCheck and linting
1. Real-World Automation
    1. File and System Automation
        - Backups and archiving
        - Monitoring changes
        - Cleanup jobs
    1. System and Network Tasks
        - Service checks
        - Network monitoring
        - Deployment helpers
    1. Scheduling and Integration
        - `cron`
        - Timers (`systemd` timers)
        - CI/CD hooks
