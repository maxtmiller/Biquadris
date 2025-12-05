# Biquadris

**Biquadris** is a modern, multiplayer adaptation of Tetris, developed as the final project for **CS246: Object-Oriented Software Development** at the University of Waterloo. Biquadris allows players to experience the classic puzzle action while introducing new strategic elements, making it both familiar and innovative.

The game features both **graphical (X11)** and **text-based** displays, a modular and extensible architecture, and advanced gameplay mechanics that enhance the classic Tetris experience. It demonstrates object-oriented principles, design patterns, and modern C++20 programming techniques.

## 🚀 Features

### 🎮 Core Gameplay
Biquadris delivers a classic falling-block puzzle experience with smooth movement controls, including left, right, down, rotation, and drop. The game supports both a graphical X11 display and a text-based terminal display, ensuring it runs in a wide variety of environments. Players can choose from six difficulty levels and enjoy gameplay featuring nine distinct block types. The game also includes a two-player competitive mode, where players can influence each other’s boards through various interactive negative effects.

### ⭐ Bonus Game Mechanics
Beyond the core gameplay, Biquadris introduces several enhanced mechanics. At higher levels, obstacles appear on the board to increase the challenge. Players can strategically store a piece using the hold-block mechanic or choose to skip a block, incurring a point penalty. Additionally, a new “Plus” (‘+’) block shape expands the traditional block set, adding fresh tactical possibilities.

## 🧩 Architecture

Biquadris is developed using modern C++20 features and solid object-oriented design principles. Its architecture emphasizes modularity, extensibility, and clean separation of responsibilities throughout the codebase. The project uses several well-established software design patterns. The Template Method Pattern structures the level system, where the base level class defines the overall block-generation algorithm while subclasses customize the specific behavior. A Factory Pattern is used to dynamically create blocks and levels based on gameplay conditions. Rendering follows the Strategy Pattern, allowing the board to switch between text-based and graphical displays.

### 📐 UML Overview
<img width="1000" height="800" alt="uml-final" src="https://github.com/user-attachments/assets/97aadd0c-0c0d-45dd-9c0b-607af45d7ce1" />

## 🖥️ Gameplay Previews

### 🎨 Graphical Display (X11)
<img width="1000" height="800" alt="Base Game Graphics Display" src="https://github.com/user-attachments/assets/7df8dbba-0b41-4f50-acaa-85e7c7883a70" />

### 🔥 Bonus Features in Action
<img width="1000" height="800" alt="Bonus Features Graphics Display" src="https://github.com/user-attachments/assets/a0f26bd0-ac93-497b-8932-d9e8f4f5ab51" />

### 📄 Text Display Mode
<div style="display: flex;">
  <img width="350" height="700" alt="Base Game Text Display" src="https://github.com/user-attachments/assets/1124fc7e-ec9c-46cd-bcfc-d5a2138b16f0" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img width="350" height="700" alt="Bonus Features Text Display" src="https://github.com/user-attachments/assets/d3bc89ab-c05d-4da1-bf97-da321ae2e5b2" />
</div>

## 🔧 Setup (Linux support only)

### Instructions:
1. Clone repository:

   ```bash
     git clone https://github.com/maxtmiller/Biquadris.git
     cd Biquadris
   ```

2. Run (graphics + text display):
   
   ```bash
     ./biquadris
   ```

### CMD Options:
- `-text` Run with text display
- `-startlevel [0-5]` Set the starting level
- `-sequencefile<1,2> [file.txt]` Set block sequence from file
- `-seed [num]` Set random seed for block generation
- `-enablebonus` Enable bonus features
