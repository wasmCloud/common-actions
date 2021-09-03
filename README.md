# Common Actions
Common GitHub actions for use across wasmCloud repositories

| Name | Purpose | Options |
|---|---|---|
| [crates-release](./crates-release) | Authenticates with crates.io and publishes a crate. | `working-directory`: Used to define the path of the crate, useful if it's not located at the root of a repository (default `./`)<br>`crates-token`: Authentication token for crates.io (required)|
| [install-cross](./install-cross) | Installs the cross-compilation tool `cross` from a branch that supports macos targets | N/A |
| [install-wash](./install-wash) | Installs the wasmCloud shell, [wash](https://github.com/wasmcloud/wash) | N/A |
| [run-nats](./run-nats) | Runs NATS for integration testing | `options`: Used for defining NATS options, e.g. `-js` to enable JetStream (not required) |
| [run-redis](./run-redis) | Runs `redis-server` for integration testing | `port`: Port to expose redis-server over (default `6379`) |
| [rust-check](./rust-check) | Checks formatting, clippy linting, and runs `cargo build` and `cargo test` on a rust project |  `working-directory`: Used to define the path of the project, useful if it's not located at the root of a repository (default `./`)|