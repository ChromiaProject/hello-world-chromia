# Hello World Chromia dApp

A simple Hello World decentralized application built with Rell on the Chromia blockchain.

## Project Structure

```
hello-world-chromia/
├── chromia.yml                 # Project configuration
└── src/
    ├── main.rell               # Main module with hello_world query
    └── test/
        ├── arithmetic_test.rell  # Basic arithmetic tests
        └── data_test.rell        # Data operation tests
```

## Getting Started

### 1. Start the Node

Start a local Chromia node:

```bash
chr node start
```

This command starts a node with your blockchain running locally. The blockchain `my_rell_dapp` defined in `chromia.yml` will be started with `main` as its entry point.

The terminal will display info messages about committed blocks and transactions.

### 2. Query the dApp

Open a **new terminal** (keep the node running in the first terminal) and run:

```bash
chr query hello_world
```

You should see the following output:

```
"Hello World!"
```

> **Note:** If your node is running on a URL other than the default `http://localhost:7740`, use the `--api-url` option:
> ```bash
> chr query hello_world --api-url http://your-node-url:port
> ```

### 3. Update the Name (Optional)

You can change the greeting name using the `set_name` operation:

```bash
chr tx set_name "Chromia"
```

Then query again to see the updated message:

```bash
chr query hello_world
```

Output:

```
"Hello Chromia!"
```

## Running Tests

Run the test suite using:

```bash
chr test
```

This will execute all tests in the `src/test/` folder:
- `arithmetic_test.rell` - Basic arithmetic assertions
- `data_test.rell` - Tests for the `set_name` operation

## Project Configuration

The `chromia.yml` file contains the project configuration:

```yaml
blockchains:
  my_rell_dapp:        # Blockchain name
    module: main       # Entry point module
compile:
  rellVersion: 0.13.14 # Rell language version
database:
  schema: schema_my_rell_dapp
test:
  modules:
    - test             # Test module location
```

