# CLAUDE.md

This file provides guidance to Claude Code when working with this simple games repository.

## Project Overview

This is a monorepo containing a collection of simple browser-based games. Each game is implemented in its own subdirectory and may use different programming languages and frameworks that target web browsers.

## Project Structure

```
/
├── README.md           # Main project documentation
├── LICENSE            # Apache License 2.0
├── CLAUDE.md          # This file
└── game-name/         # Individual game directories
    ├── README.md      # Game-specific documentation
    ├── index.html     # Game entry point
    └── ...            # Game implementation files
```

## Directory Naming Convention

- Game directories use lowercase names
- Only alphanumeric characters allowed
- Words separated by dashes (e.g., `tic-tac-toe`, `memory-game`)

## Browser Compatibility

- Target all modern browsers
- No need to support legacy browsers

## Shared Assets

- Avoid putting shared assets in this repository
- Each game should be self-contained within its directory
- If assets are needed, prefer external CDNs or inline resources

## Development Guidelines

### Game Structure
Each game should be organized within its own directory with:
- `index.html` as the main entry point
- Game-specific build tools and configuration as needed
- Individual README.md with setup and running instructions

### Technology Choices
- HTML/CSS/JavaScript for simple games
- Languages that compile to WebAssembly are welcome
- Build tools decided on a game-by-game basis
- No enforced framework or tooling standards

### Code Quality
- No specific linting requirements yet
- Follow standard practices for the chosen technology
- Keep games simple and focused

## Adding New Games

1. Create a new directory with a descriptive, dash-separated name
2. Implement the game within that directory
3. Add a README.md explaining how to run the game
4. Update the main README.md to list the new game

## Contributing

- Each game may use different technologies and practices
- Follow the existing patterns within each game directory
- Ensure games run in modern web browsers
- Keep implementations simple and educational