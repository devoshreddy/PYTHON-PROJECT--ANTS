Langton's Ant — Python Simulation
An interactive visualization of Langton's Ant, a two-dimensional cellular automaton that demonstrates how simple local rules can produce complex, emergent patterns.
Features
- Interactive grid-based simulation
- Ant turns, flips the current cell, and moves according to the two-color rules
- Live step and black-cell counters
- Pause/resume, single-step, reset, and speed controls
- Configurable grid dimensions and cell size
Rules
1. If the ant is on a white cell, it turns right, changes the cell to black, and moves forward one cell.
2. If the ant is on a black cell, it turns left, changes the cell to white, and moves forward one cell.
3. The grid wraps at its edges (toroidal boundary).
Requirements
- Python 3.10 or later recommended
- Pygame
Setup and run
python -m venv .venv
# Windows:
.venv\\Scripts\\activate
# macOS/Linux:
source .venv/bin/activate

python -m pip install -r requirements.txt
python langtons_ant.py
Controls
Key	Action
SPACE	Pause / resume
RIGHT	Advance one step while paused
R	Reset
UP / DOWN	Increase / decrease speed
ESC or Q	Quit


Command-line options
python langtons_ant.py --width 120 --height 90 --cell-size 7 --speed 800
python langtons_ant.py --no-grid
Project structure
langtons-ant-project/
├── langtons_ant.py
├── requirements.txt
├── README.md
└── .gitignore
Algorithm (pseudocode)
IF current cell is black:
    turn left
    make current cell white
ELSE:
    turn right
    make current cell black
move forward one cell
repeat
Learning outcomes
- Understand cellular automata and rule-based systems
- Practice sets, tuples, classes, and modular programming in Python
- Observe emergent behavior from simple deterministic rules
- Explore simulation loops and real-time graphics with Pygame
GitHub upload
1. Create a new repository on GitHub (for example, langtons-ant-python).
2. Upload langtons_ant.py, README.md, requirements.txt, and .gitignore, or push the project folder with Git.
3. Copy the repository URL from the GitHub page and share it as your project link.
License
This project is provided for educational use. You may add a license file if your course or institution requires one.
