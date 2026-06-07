# Bandit - Room 12

## Concept
Decode a hexdump file and decompress a chain of 
files compressed in multiple formats.

## Steps
1. `xxd -r -p` to convert the hexdump back to binary
2. `file` to identify the format
3. Decompress according to the format (`gunzip`, `bunzip2`, `tar -xf`)
4. Repeat until you get an ASCII file

## Useful commands
- `file` — identify file type
- `xxd -r -p` — decode a hexdump
- `gunzip`, `bunzip2`, `tar -xf` — decompress
- `mktemp -d` — create a temporary folder in /tmp
