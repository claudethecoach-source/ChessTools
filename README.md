# St. Catharines Chess Club Weekly Manager

A lightweight, browser-based tool for running a weekly chess club session. It helps club organizers manage player registrations, attendance, Swiss-style pairings, score reporting, and a continuing King of the Hill ladder.

This project is a single-page web application built with HTML, CSS, and JavaScript. It runs entirely in the browser and stores club data locally in the browser's local storage, so there is no database or server setup required.

## Features

- Player roster management
- Manual Elo entry or Chess.com username-based rating lookup
- Attendance check-in for the weekly session
- Swiss/Elo-proximity pairing generation
- Manual pairing override for custom boards
- Round result completion and rating updates
- King of the Hill standings and win streak tracking
- Dark mode and light mode support
- JSON export/import for backup and restoration
- Club data reset controls for clean weekly resets

## Project files

- [chess_club_weekly_manager.html](chess_club_weekly_manager.html) — main application
- [mylogo.jpg](mylogo.jpg) — club logo used in the UI
- [MIT-license.txt](MIT-license.txt) — project license
- [St. Catharines Chess Club Manager - User & Technical Guide.pdf](St.%20Catharines%20Chess%20Club%20Manager%20-%20User%20%26%20Technical%20Guide.pdf) — detailed user and technical guide

## Getting started

### Option 1: Open directly in a browser

1. Open [chess_club_weekly_manager.html](chess_club_weekly_manager.html) in a browser.
2. If you want the app to behave like a normal web page, use a local web server instead of opening the file directly.

### Option 2: Run a local web server

From the project folder:

```bash
cd "G:\My Drive\Projects\ChessTools\ClubManager"
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/chess_club_weekly_manager.html
```

## How to use it

1. Add players to the roster.
2. Choose either a manual Elo rating or a Chess.com username.
3. Mark players as checked in for the current session.
4. Generate weekly Swiss pairings.
5. Enter results for the round.
6. Complete the round to update club ratings and standings.
7. Review the King of the Hill leaderboard.
8. Use the gear icon to export/import data or reset the round history.

## Data storage

The app stores state in the browser using `localStorage`. This means:

- your data remains on the browser/device where it is used
- no external database or backend is required
- exporting the data as JSON is recommended before resetting or migrating the app

## Notes

- The app is designed for a club environment and is intentionally simple to run without installation.
- A fallback placeholder logo is used if the club image is missing.
- The project is released under the MIT license.

## License

This project is licensed under the MIT License. See [MIT-license.txt](MIT-license.txt) for the full text.
