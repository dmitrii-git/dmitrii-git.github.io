Git Commander – Retro GitHub Explorer
Git Commander is a retro‑styled Norton Commander–inspired GitHub explorer built entirely in HTML, CSS, and JavaScript.
It lets you browse a user's repositories and navigate through repo file structures using keyboard‑driven navigation, just like classic DOS file managers.

The interface emulates a vintage terminal aesthetic while interacting with the GitHub API in real time.

⭐ Features
Two‑panel layout

Left: Repositories

Right: Files & folders inside the selected repository

Keyboard‑first navigation

Move, open, switch panels, go up directories

GitHub API integration

Fetches repositories and repo contents dynamically

Retro terminal UI

Courier font, deep‑blue palette, classic NC‑style panels

Command line mode

:open <repo>

:cd <repo>

:cd ..

:clear

Open files directly on GitHub

Clicking or pressing Enter on a file opens it in a new tab

Zero dependencies

Pure HTML + CSS + JavaScript

🎮 Keyboard Controls
Action	Key
Move selection	↑ / ↓
Switch panel	← / →
Open repo / folder / file	Enter
Go up one directory	Backspace
Open command line	:
Help popup	F1
🧪 Commands
Inside the command line (:):

Command	Description
help	Show available commands
open	Open a repository
cd	Same as open
cd ..	Go up one directory
clear	Clear the right panel
🚀 Getting Started
Clone or download the project, then simply open the HTML file in your browser:

bash
git clone https://github.com/<your-repo>/git-commander
cd git-commander
open index.html
No build steps. No dependencies. Just open and go.

🧩 How It Works
Git Commander uses the GitHub REST API:

GET /users/:user/repos – loads repositories

GET /repos/:user/:repo/contents/:path – loads files and folders

The UI updates dynamically as you navigate, highlighting the active panel and selected item.

🛠 Configuration
At the top of the script, set the GitHub username to browse:

js
const user = "dmitrii-git";
Change it to any public GitHub username.

📂 Project Structure
Code
index.html
└── Retro UI
    ├── Two-panel layout
    ├── Command line input
    └── GitHub API integration
Everything is contained in a single HTML file.

🧭 Roadmap Ideas
File preview panel

Search inside repositories

Theme switcher (light/dark/retro)

Bookmark favorite repos

Local caching

📜 License
MIT License — free to use, modify, and build upon.
