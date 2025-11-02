# Chip-8-Emulator
Group Name: Chips-Ahoy

Group Member Names and NetID:

Dev Shah---dshah219

Vaibhav Goel---vkgoel2

## Project Introduction
The goal of our project is to build a fully functional Chip-8 (Nintendo Entertainment System) emulator using Rust. CHIP-8 is a simple, interpreted programming language used on early microcomputers from the 1970s, making it an excellent foundation for learning about how emulators work at a low level. We chose this project because it’s a challenging yet approachable way to explore computer architecture concepts, low-level programming, and Rust’s memory safety guarantees, which are all valuable skills that we are interested in developing.

Our goals and objectives include:

---Understand the inner workings of CPU emulation, memory management, and instruction decoding.

---Build a fully functional CHIP-8 emulator capable of running original CHIP-8 games (e.g., Pong, Space Invaders).

---Strengthen our knowledge of systems programming and Rust’s safety and concurrency features.

## Technical Overview
### 1. CPU/Instruction Decoder---Implement the CHIP-8 instruction set.
---A program counter, stack, registers (V0–VF), and index register.

---Opcode fetching, decoding, and execution logic.

---Timers (delay and sound timers) that update at 60 Hz.

### 2. Memory Management – 4KB memory model divided into reserved system space, font data, and program data---Finish by Checkpoint 1
---Handles loading CHIP-8 ROMs into memory.

---Stores fonts and sprites used by CHIP-8 programs.

### 3. Display System – A monochrome 64x32 pixel display.---Finish By Checkpoint 2
---We’ll use a Rust graphics library to draw pixels to the screen.

---Includes methods for clearing and updating the screen.

### 4. Input System – Emulates the 16-key hexadecimal keypad.---Finish by Checkpoint 3
---Maps modern keyboard inputs to CHIP-8 keys.

---Supports input polling to detect presses and releases.

### 5. Main Emulator Loop – Fetches, decodes, executes instructions, updates timers, and redraws the display each frame.

##Possible Challenges
###Implementing the instruction set correctly:
---The CHIP-8 instruction set has around 35 opcodes, and minor mistakes in bit masking or decoding logic can cause unexpected behavior. Testing and debugging the CPU will likely be time-consuming.

###Integrating a graphics/UI crate:
---Choosing and learning to use a windowing/graphics crate such as minifb or sdl2 will be a challenge, particularly when synchronizing rendering speed with the emulator’s timing system.
