
---

# MyNetcat

MyNetcat is a simple implementation of the netcat (nc) networking utility, written in C. This tool can be used for reading from and writing to network connections using TCP or UDP protocols. 

## Features

- **TCP/UDP Support**: Handle both TCP and UDP connections.
- **Port Scanning**: Scan for open ports on a target host.
- **Data Transfer**: Send and receive data over network connections.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/WasiimSheb/MyNetcat.git
    ```
2. Navigate to the project directory:
    ```bash
    cd MyNetcat
    ```
3. Compile the source code:
    ```bash
    make
    ```

## Usage

```bash
./mynetcat [OPTIONS] [hostname] [port]
```

### Options

- `-l`: Listen mode, for inbound connects.
- `-u`: UDP mode.
- `-p <port>`: Local port number.
- `-e <program>`: Program to execute after connect.

### Examples

- **Start a simple TCP server**:
    ```bash
    ./mynetcat -l -p 1234
    ```
- **Connect to a TCP server**:
    ```bash
    ./mynetcat 192.168.0.1 1234
    ```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.

---

Feel free to customize this template further to suit your specific needs.
