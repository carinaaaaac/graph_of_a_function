#  Graphical Function Calculator

An interactive, custom-built mathematical function plotter and evaluator written in **C++**. This application parses raw string inputs of mathematical functions, converts them using algorithmic logic, and renders their graphs on a dynamic Cartesian coordinate system.

##  Features

* **Custom Expression Parser:** Implements the **Shunting-yard algorithm** (using custom Stack and Queue data structures) to convert Infix mathematical expressions to Postfix (Reverse Polish Notation) for real-time evaluation.
* **Advanced Graphing:** Plots single or multiple functions simultaneously with automatic scaling, min/max normalization, and discontinuity handling.
* **Interactive Pan & Zoom:** Users can interactively explore the graph using on-screen controls to zoom in/out and pan across the axes.
* **Calculus Operations:** * Computes the **definite integral** of a function on a specified interval.
  * Automatically calculates and draws **horizontal and vertical asymptotes**.
* **Syntax Evaluator:** Includes a robust error-checking system that validates user input (e.g., checking for unbalanced parentheses or invalid operator placements) before attempting to plot.
* **Customizable UI:** Features a fully interactive graphical menu built with `graphics.h`. It includes a settings panel where users can switch the language (English/Romanian) and change the accent color. Preferences are persistently saved in a binary file (`settings.dat`).

##  Technologies & Libraries

* **Language:** C++
* **Graphics Library:** `graphics.h` / WinBGIM (Borland Graphics Interface for Windows)
* **Core Concepts:** Data Structures (Linked Lists, Stacks), Algorithmic Parsing, File I/O (Binary serialization), Numerical Methods.

##  Project Structure

* `main.cpp`: The entry point of the application.
* `func.h`: The core mathematical engine. Contains the Shunting-yard algorithm, expression validation, integral calculus, and asymptote logic.
* `drawgraph.h`: Handles the rendering logic, including the coordinate axes, graph plotting, and the Pan/Zoom interaction loop.
* `settings.h`: Manages user preferences (Language & Theme) and handles saving/restoring states using `std::fstream`.
* `menu.h` & `menu1.h`: Manage the graphical user interface, user input capturing, and screen transitions.

##  How to Run

1. **Prerequisites:** You need a C++ IDE configured with the **WinBGIM** library (e.g., Code::Blocks with WinBGIM setup).
2. Clone this repository:
   ```bash
   git clone [https://github.com/carinaaaaac/your-repo-name.git](https://github.com/carinaaaaac/your-repo-name.git)
