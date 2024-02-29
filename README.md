# dll_unhook


`dll_unhook` is a Rust-based tool designed for bypassing EDR and AV hooks within Windows systems. Utilizing advanced in-memory disassembly techniques, this project aims to identify and revert modifications made to DLLs by EDR/AV software, enabling researchers to execute original, unaltered code.

## Features

- **In-memory Disassembly**: Dynamically identifies hooks and restores original DLL code blocks without relying on direct system calls or vulnerable APIs.
- **Rust for Security**: Leverages Rust's memory safety features to minimize risks associated with low-level memory manipulation.
- **EDR/AV Evasion**: Bypasses common detection mechanisms, facilitating undetected execution of security research tools and payloads.

## Usage
Run dll_unhook from the command line, specifying the target DLL or process as an argument:

```shell
cargo run --release -- <TARGET_PROCESS_OR_DLL>
```

## Prerequisites

- Rust programming environment
- Windows system for analysis
- Basic understanding of EDR/AV hooking mechanisms

## Installation

1. Clone the repository:
   ```shell
   git clone https://github.com/yourusername/dll_unhook.git
   ```
   
2. Navigate to the project directory and build the project:
   ```shell
   cd dll_unhook
   cargo build --release
   ```


