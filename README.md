#  Authentication-Based Unlocking System using 8051

This project demonstrates a Password-Protected Door Lock System using an AT89C51 microcontroller, 4x3 matrix keypad, 16x2 LCD, and DC motors to simulate a door mechanism. The system grants access upon correct password entry and denies it otherwise.

# Features

- 4-digit password input using a matrix keypad
- LCD display for system messages and feedback
- DC motors to simulate door opening and closing
- Access granted/denied logic based on password verification
- Simple user interface with '*' masking

# File Structure

| File Name                                      | Description                               |
|-----------------------------------------------|-------------------------------------------|
| `authentiaction based unlocking system.c`      | Source code in embedded C for 8051        |
| `Authentication based unlocking system.hex`    | HEX file for flashing to the microcontroller |
| `Authentication based unlocking system.uvproj` | Keil µVision project file                 |

# Hardware Requirements

- AT89C51 Microcontroller
- 16x2 LCD
- 4x3 Matrix Keypad
- 2 DC Motors (for door simulation)
- L293D Motor Driver IC
- Power supply
- Connecting wires, breadboard or PCB

# How It Works

1. On startup, LCD displays “PSWD PROTECTION SYSTEM”.
2. The user is prompted to "ENTER PASSWORD".
3. The system reads 4 digits from the keypad and masks input with '*'.
4. If the entered password is correct (`1513`), motors activate to open the door.
5. A delay simulates time for access.
6. The system automatically closes the door and resets.
7. If the password is incorrect, it displays "ACCESS DENIED".

# Default Password

```text
1513
