# Simple Key-Value Store

A basic in-memory key-value store implemented in Go, compatible with Redis CLI.

## Features

- Store and retrieve key-value pairs.
- Thread-safe operations using concurrency control.
- Compatible with Redis CLI for easy interaction.
- Runs on the default Redis port (6379).

## Redis CLI Compatibility

This key-value store is designed to work with the Redis CLI, allowing you to use familiar Redis commands to interact with the store.

## Installation

### Installing Redis CLI

#### On Ubuntu/Debian:
```
sudo apt-get update
sudo apt-get install redis-tools
```

#### On macOS (using Homebrew):
```
brew install redis
```

#### On Windows:
1. Download the Redis package from the official Redis website.
2. Extract the package and add the Redis directory to your system PATH.

### Installing and Running the Key-Value Store

1. Clone the repository:
   ```
   git clone https://github.com/achint227/kvstore.git
   ```
2. Navigate to the project directory:
   ```
   cd kvstore
   ```
3. Stop the Redis Server (if running):
   * macOS:
     ```
     brew services stop redis
     ```
   * Linux:
     ```
     sudo systemctl stop redis
     ```
   * Windows:
     Open the Task Manager, go to the “Services” tab, find the Redis service, right-click on it, and select “Stop”.
     
4. Run the project:
   ```
   go run *.go
   ```

## Usage

Once the server is running, you can use Redis CLI to interact with it:

```
redis-cli
```

The server runs on the default Redis port (6379), so you don't need to specify a port when connecting with redis-cli.

Example commands:
- SET key value
- GET key

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
