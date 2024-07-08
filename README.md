
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

## Implementation Details

### src Directory

1. **q1**:
   - **Description**: Implemented basic TCP client functionality.
   - **Details**: Established a connection to a server and sent/received data.

2. **q2**:
   - **Description**: Implemented basic TCP server functionality.
   - **Details**: Listened for incoming connections and handled client communications.

3. **q3**:
   - **Description**: Added UDP client functionality.
   - **Details**: Sent and received data using the UDP protocol.

4. **q4**:
   - **Description**: Added UDP server functionality.
   - **Details**: Listened for incoming UDP datagrams and responded appropriately.

5. **q5**:
   - **Description**: Implemented port scanning capabilities.
   - **Details**: Scanned specified ports on a target host to check for open ports.

6. **q6**:
   - **Description**: Enhanced error handling and robustness.
   - **Details**: Improved the stability of the application by handling various edge cases and errors.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.
## Contact

ShifaaKhatib28@gmail.com
Wasimshebalny@gmail.com
