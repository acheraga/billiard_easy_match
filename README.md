# Billard Game Manager (`ASSIST WITH IA CLAUD AI and COPILOT`)

## Overview

This file implements a billiard game manager using Vue.js (CDN version).  
It provides a modern, responsive interface for managing two-player billiard matches, including timers, extensions, score tracking, and player switching.

## Features

- **Two Players**: Each player has a name, match score, and extension status.
- **Timer Management**: Per-turn timer, configurable duration, pause/resume/stop controls.
- **Extension**: Each player can use a time extension once per game.
- **Double Time**: After the break shot, the active player can play with double time.
- **Break Shot Handling**: Valid or invalid break determines who plays next and with double time.
- **Score Tracking**: Increment/decrement match score, automatic new game on win.
- **Player Switching**: Manual switch button to pass the turn and reset the timer.
- **Game Controls**: Start, pause, resume, stop timer, new game, reset match.
- **Configuration**: Set player names, shot time, extension time before starting the timer.
- **Responsive Design**: Adapts to mobile and desktop screens.

## Main Components

- **Header**: Displays match score, current game number, and game status.
- **Configuration Section**: Allows setting player names, shot time, and extension time.
- **Player Cards**: Shows player info, timer, score controls, and extension button.
- **Central Controls**: Game actions (start, pause, resume, stop, switch player, new game, reset match).
- **Break Handling**: Special UI and logic for the break shot phase.

## Usage

1. **Configure** player names, shot time, and extension time.
2. **Start the game**: The break shot phase begins, with no time limit.
3. **Validate break**: Choose if the break is valid or not.
   - Valid: Same player continues with double time.
   - Invalid: Opponent plays with double time.
4. **Start timer**: Begin the turn timer for the active player.
5. **Use extension**: Each player can use their extension once per game.
6. **Switch player**: Use the button to manually pass the turn and reset the timer.
7. **Score tracking**: Use + and - buttons to update match scores.
8. **New game**: Starts a new game, alternates the breaking player.
9. **Reset match**: Resets all scores and states.

## Technical Notes

- **Vue.js**: Uses Vue 3 via CDN (`vue.global.js`).
- **No build step**: Can be run directly in the browser.
- **Single file**: All logic, template, and styles are in one HTML file.

## Customization

- To use in a Vue CLI or Vite project, migrate the template, script, and styles into a `.vue` component.
- Extend features as needed (e.g., add win conditions, more statistics, etc.).

## Author

Abdelhamid (location: `/home/abdelhamid/Documents/billard/test2.html`)
