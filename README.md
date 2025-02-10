# custom-lc3
My custom implementaiton of the lc3 vm.

The base lc3 vm is implemeted.

Currently the below additions have been made:

# Custom Opcodes
| Opcode  | Instruction | Description |
|---------|------------|-------------|
| 0xE8    | NOP        | No Operation |
| 0xE9    | CLR R0     | Clears the specified register (sets to 0) |
| 0xEA    | INC R0     | Increments the specified register by 1 |
| 0xEB    | DEC R0     | Decrements the specified register by 1 |

# Custom System Calls
| Trap Code | Instruction   | Description |
|-----------|--------------|-------------|
| 0x26      | TRAP_PUTHEX  | Prints a number in hexadecimal format |
| 0x27      | TRAP_RND     | Generates a random number between 0 and R0 |
| 0x28      | TRAP_GETSTR  | Reads an entire string from input |
| 0x29      | TRAP_SLEEP   | Pauses execution for a specified duration (in milliseconds) |

## TODO
- [x] Add Custom Opcodes
- [ ] Implement Debugger (Breakpoints, Step-by-Step Execution)
- [ ] Implement Web-Based LC-3 VM (Run in Browser)
- [ ] Implement Simple Game in LC-3 Assembly (Snake, Pong)
- [ ] Implement JIT Compilation
- [ ] Custom OS for LC-3 (Task Switching, File System)
