#  Ape Maze Simulation (POSIX Threads)

A **multi-threaded simulation of ape families collecting bananas in a maze**, implemented in **C using POSIX threads (pthreads) on Linux**.  
The project models concurrent behaviors between different ape roles while managing shared resources and synchronization in a dynamic maze environment.

Developed for the **Real-Time Applications & Embedded Systems (ENCS4330)** course at **Birzeit University**.

---

# Project Overview

The simulation represents a maze environment where **ape families interact concurrently** while collecting bananas.

Each ape role behaves differently:

- **Female apes** navigate the maze and collect bananas.
- **Male apes** protect baskets containing collected bananas.
- **Baby apes** attempt to steal bananas during fights.
- **Conflicts and fights** may occur between apes over bananas.

The simulation ends when predefined conditions are reached, such as exceeding banana thresholds or running for a maximum amount of time.

---

#  Key Features

- Multi-threaded architecture using **POSIX threads (pthreads)**
- Concurrent simulation of multiple ape families
- **Thread synchronization** for shared resources (baskets, bananas)
- Dynamic **maze environment** with obstacles and banana distribution
- **Fight mechanics** between apes
- Energy management and withdrawal conditions
- **Graphical visualization using OpenGL**
- Configurable simulation parameters using external files

---

#  Project Structure

```
pthreads-ape-maze-simulation
│
├── src/            # Source code
│   ├── main.c
│   ├── maze.c
│   ├── female_ape.c
│   ├── male_ape.c
│   ├── baby_ape.c
│   ├── fight.c
│   └── simulation_threading.c
│
├── include/        # Header files
│
├── config/         # Simulation configuration
│   ├── arguments.txt
│   ├── maze.txt
│   └── menu.txt
│
├── results/        # Simulation outputs
│
├── Makefile
└── README.md
```

---

# Technologies Used

- **C Programming Language**
- **POSIX Threads (pthreads)**
- **Linux / Unix Environment**
- **OpenGL (graphics visualization)**
- **Makefile build system**

---

#  Build Instructions

Compile the project using:

```bash
make
```

---

# Run the Simulation

Run the program using:

```bash
./bin/ape_simulation config/arguments.txt
```

Simulation parameters (maze size, number of apes, thresholds, etc.) are defined in the configuration files.

---

# Concepts Implemented

This project demonstrates:

- **Multithreaded programming**
- **Thread synchronization**
- **Shared resource protection**
- **Concurrent system simulation**
- **Real-time behavior modeling**
- **Modular C program architecture**

---

# 👩‍💻 Author

**Leen Ahmad**  
Computer Engineering Student  
Birzeit University
