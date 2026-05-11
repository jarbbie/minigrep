# minigrep

A lightweight, command-line search tool built in Rust. This is my implementation of the guided project from Chapter 12 of [*The Rust Programming Language*](https://doc.rust-lang.org/book/ch12-00-an-io-project.html).

`minigrep` searches for a specific string of text within a file and prints the matching lines to the console—similar to the classic `grep` tool.

## Features

* **File Searching:** Quickly find specific strings within text files.
* **Case Sensitivity:** Supports both case-sensitive (default) and case-insensitive searching.
* **Standard Error Handling:** Gracefully handles missing files, permission issues, and missing arguments, printing errors to `stderr` instead of `stdout`.
* **Test-Driven:** Includes unit tests and integration tests for core logic.

## Prerequisites

To run this project, you will need to have [Rust and Cargo installed](https://www.rust-lang.org/tools/install)

## Installation & Build

Clone the repository and navigate into the project directory:

```bash
git clone [https://github.com/jarbbie/minigrep.git](https://github.com/jarbbie/minigrep.git)
cd minigrep
```

## How to use

```bash
# Case-sensitive Search
cargo run -- <query> <file_path>

# Case-insensitive search p.s. IGNORE_CASE value could be anything
IGNORE_CASE=1 cargo run -- <query> <file_path>
```

**query**: Word to find within line
**file_path**: Path to file to find specific word

You can try
`cargo run -- nahhh generation_downfall.txt`
or try
`cargo run -- with generation_downfall.txt`
for multiple lines grep
