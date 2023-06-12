# File Compressor in Rust
Simple Rust program that compresses files using gzip compression. It's a lightweight tool that can be used standalone or as part of a larger data processing pipeline.

## About

The Rust script reads a source file, compresses it using gzip, and writes the compressed data into a target file. It also prints out the sizes of the original and compressed files, along with the time taken to perform the compression.

## Prerequisites

- Rust Programming Language
- flate2 crate

## Installation

Before you can run this program, you need to have Rust installed on your machine. If you don't have Rust installed, follow the instructions [here](https://www.rust-lang.org/tools/install) to install it.

You also need to add `flate2` crate to your Rust project. Add the following to your `Cargo.toml` file:

```toml
[dependencies]
flate2 = "1.0.20"
```

## Usage

To use the script, pass two arguments to the program: the source file and the target file. For example:

```bash
cargo run source target
```

The source file is the file you wish to compress, and the target file is where the compressed data will be stored. The script will then compress the source file and save the result in the target file. It will also print the sizes of the original and compressed files and the time it took to perform the compression.

Please note: This script does not handle errors gracefully - it will panic when it encounters an error, such as if a file can't be opened or written. In a production setting, you may want to modify the script to handle these errors more elegantly.


## Contributing

Contributions, issues and feature requests are welcome.