<p align="center">
    <img width=30% src="https://github.com/robertmartin8/PyGameofLife/blob/master/media/logo.gif">
</p>

<h1 align="center"> PyGameofLife </h1>

<!-- buttons -->
<p align="center">
    <a href="https://www.python.org/">
        <img src="https://img.shields.io/badge/python-v3-blue.svg?style=for-the-badge"
            alt="python"></a> &nbsp;
    <a href="https://opensource.org/licenses/MIT">
        <img src="https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge"
            alt="MIT license"></a> &nbsp;
    <a href="https://github.com/robertmartin8/PyPortfolioOpt/graphs/commit-activity">
        <img src="https://img.shields.io/badge/Maintained%3F-yes-blue.svg?style=for-the-badge"
            alt="maintained"></a> &nbsp;
</p>
# PyGameofLife

## Overview
PyGameofLife is a simple implementation of Conway’s Game of Life using Python. It features a command-line interface that allows users to generate and customize animations of cellular automata. The focus is on readability and simplicity rather than performance optimization.

## Installation

### Dependencies
PyGameofLife requires `numpy` and `matplotlib`. Install them using:
```bash
pip install numpy matplotlib
```

### Clone the Repository
To get the code, run:
```bash
git clone https://github.com/robertmartin8/PyGameofLife
cd PyGameofLife
```

## Running the Simulation
To start the simulation with the default settings, run:
```bash
python life.py
```
This will generate an animation saved as `infinite.gif` in the current directory.

## Command-Line Options
To see all available options, run:
```bash
python life.py --help
```

### Main Options
- `--universe-size X,Y`  → Set the grid size.
- `-seed SEED_NAME` → Choose a predefined seed pattern.
- `-n N` → Define the number of iterations.
- `-interval TIME` → Set the time interval (in ms) between updates.
- `-quality DPI` → Adjust the image quality.
- `-cmap COLOR_MAP` → Change the color scheme.
- `--seed-position X,Y` → Set the initial position of the seed.

## Example Commands
Run the simulation with a predefined seed:
```bash
python life.py -seed diehard
```
Run with a smaller grid and custom colors:
```bash
python life.py -seed beacon --universe-size 6,6 --seed-position 1,1 -cmap plasma_r
```

## Customizing Seeds
Seeds are predefined patterns. The available options include `diehard`, `boat`, `r_pentomino`, `beacon`, and more. To add a new seed, modify the `seeds` dictionary in `life.py`.

## About
This project is designed as an educational tool to demonstrate cellular automata using Python. The code prioritizes readability and intuitive design over efficiency.


