# Reflection on Module 6

<details>
<summary><b>Milestone 1</b></summary>

## Milestone 1 Reflection

### Commit 1 Reflection Notes

#### handle_connection Function Analysis
- Uses `BufReader` to efficiently read data from the TCP stream
- Reads lines until an empty line is encountered (end of HTTP request header)
- Collects request lines into a vector for inspection

#### HTTP Request Structure
Typical request contains:
- Method (GET)
- Path (/)
- HTTP version
- Headers (Host, User-Agent, Accept, etc.)
- Followed by empty line

#### Key Rust Concepts Demonstrated
- TcpListener/TcpStream for network communication
- Error handling with `.unwrap()` (for simplicity)
- Iterator processing with `map()` and `take_while()`
- Buffering with BufReader for efficient IO

</details>