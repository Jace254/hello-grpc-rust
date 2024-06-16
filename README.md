# gRPC in RUST

## Pre-requisites

- Ensure you have [Rust](https://www.rust-lang.org/tools/install) installed.
- [Install](https://protobuf.dev/downloads/#release-packages) and set PROTOC on your PATH if you're on windows.
- Otherwise follow steps described [here](https://grpc.io/docs/protoc-installation/).

## Development

- Run the server with:

    ```sh
    cargo run --release --bin server
    ```

- Build the cli client and run it with these [commands](#commands) to access the server.

    ```sh
    # building the cli
    cargo build --release --bin cli
    # copy it to project root dir
    cp ./target/release/cli ./cli
    ```

### Commands

```sh
Usage: cli.exe <COMMAND>

Commands:
  add
  remove
  get
  update-quantity  
  update-price     
  watch
  help             Print this message or the help of the given subcommand(s)

Options:
  -h, --help  Print help
```
