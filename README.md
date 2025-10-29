# NES-Emulator

## Project Introduction
The goal of our project is to build a fully functional NES (Nintendo Entertainment System) emulator using Rust. We will simulate the NES hardware environment so that we can load and play classic NES games directly through our program. We chose this project because it combines low-level systems programming with emulation theory, computer architecture, and graphics programming. These are topics that we were interested in exploring, and Rust's design makes it an ideal language for a project like this one. 

Our goals and objectives include:
---Building a NES emulator capable of running simple NES games.
---Implementing the NES CPU instruction set and memory model.
---Emulate core components including the CPU, PPU (Picture Processing Unit), APU (Audio Processing Unit), and input handling.
---Render graphics output in real time and support basic user interaction.

## Technical Overview
### 1. NES Platform Setup
---Define core system structure (CPU, PPU, APU, BUS, Cartridge).

---Establish communication between these components through shared interfaces.

### 2. CPU Emulation---Finish by Checkpoint 1
#### 2.1. Getting Started
---Implement CPU registers, stack, and basic instruction cycle loop.

---Add support for basic instruction fetching and decoding.

#### 2.2. Memory Addressing Modes
---Implement all 13 addressing modes supported by the NES CPU.

#### 2.3. Full Instruction Set
---Implement remaining instructions (arithmetic, branching, flags, etc.).

---Ensure accurate cycle timing and correct flag behavior.

#### 2.4. Running First Game
---Load a simple test ROM and verify correct CPU execution.

### 3. BUS Implementation
---Create the NES bus for communication between CPU, PPU, APU, and cartridge.

---Implement read/write access and memory mirroring logic.

### 4. Cartridge Handling---Finish by Checkpoint 2
---Parse iNES file format headers.

---Load PRG (program) and CHR (character) ROMs into memory.

---Implement Mapper 0 (NROM) to test initial games.

### 5. PPU (Picture Processing Unit) Emulation---Finish by Checpoint 3
#### 5.1. PPU Registers and NMI Interrupt
---Implement control/status registers and NMI triggering.

#### 5.2. Rendering
---Render CHR ROM tiles to a window.

---Draw static backgrounds, then progress to dynamic rendering.

### 6. Joypad Input
---Map keyboard input to NES controller buttons.

---Connect input data to memory-mapped registers.

### 7. APU (Audio Processing Unit)---Finish by Checkpoint 4
---(Stretch goal) Begin implementing basic tone generation and audio channels.
