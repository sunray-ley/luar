# Luar

Luar is a Lua interpreter implemented in Rust. It aims to provide a high-performance, reliable interpreter that supports as many Lua features as possible.

## Features

- Basic capabilities for parsing, compiling, and executing Lua code

- Highly configurable with support for custom Lua standard libraries

- Purely implemented in Rust, providing high performance and safety guarantees

- Easy to embed into Rust applications

## Installation

To use Luar, you need to have Rust programming language and Cargo package manager installed. Please refer to [Rust's official website](https://www.rust-lang.org/) for installation instructions.

Use the following command in the terminal to install Luar:

```shell
$ cargo install luar
```

**Note: Luar is still under active development and will soon be installable using the above command.**

## Usage

### Command-line Interface

If you want to run an interactive Lua shell, execute the following command:

```shell
$ luar
```

To run a Lua script, execute the following command:

```shell
$ luar script.lua
```

### In Rust Applications

You can also integrate Luar into your own Rust projects. Add the following dependency in your `Cargo.toml` file:

```toml
[dependencies]
luar = "0.1"
```

In your Rust code, use the following code to load and run a Lua script:

```rust
use luar::State;

fn main() {
    let mut lua = State::new();
    lua.load("print('Hello, world!')").exec().unwrap();
}
```

Refer to the [documentation](https://docs.rs/luar) for more detailed explanations.

## Contributing

Contributions to Luar are welcome! If you have any suggestions or questions, please open an issue or pull request on GitHub.

## License

Luar is distributed under the MIT License. Please refer to the [LICENSE](https://github.com/sunray-ley/luar/blob/main/LICENSE) file for more information.
