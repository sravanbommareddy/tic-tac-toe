# 🎮 Tic-Tac-Toe Game using HTML, CSS, JavaScript & Docker

A simple and interactive Tic-Tac-Toe (X-O) web application built using **HTML**, **CSS**, and **JavaScript**, and deployed using **Docker** with the **Nginx** web server.

---

# 📌 Project Overview

This project demonstrates how to containerize a static web application using Docker.

The application consists of:

- HTML (Game UI)
- CSS (Styling)
- JavaScript (Game Logic)
- Nginx (Web Server)
- Docker (Containerization)

---

# 🚀 Features

- Two-player Tic-Tac-Toe game
- Interactive game board
- Win detection
- Draw detection
- Player turn indicator
- Game reset button
- Responsive UI
- Dockerized application
- Runs on Nginx web server

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| HTML5 | User Interface |
| CSS3 | Styling |
| JavaScript | Game Logic |
| Docker | Containerization |
| Nginx | Web Server |

---

# 📁 Project Structure

```
tic-tac-toe/
│
├── index.html
├── tic.css
├── tic.js
├── Dockerfile
└── README.md
```

---

# 🐳 Dockerfile

```dockerfile
FROM nginx

COPY . /usr/share/nginx/html
```

The Dockerfile:

- Pulls the official Nginx image.
- Copies all project files into Nginx's default web root.
- Serves the application through Nginx.

---

# ⚙️ Prerequisites

Before running the project, ensure you have:

- Docker installed
- Git installed (optional)

Verify Docker installation:

```bash
docker --version
```

---

# 📥 Clone the Repository

```bash
git clone <repository-url>

cd tic-tac-toe
```

Example:

```bash
git clone https://github.com/username/tic-tac-toe.git

cd tic-tac-toe
```

---

# 🏗️ Build Docker Image

```bash
docker build -t tic-tac-toe:v1 .
```

Verify image:

```bash
docker images
```

---

# ▶️ Run Docker Container

```bash
docker run -d \
--name tic-game \
-p 8080:80 \
tic-tac-toe:v1
```

Verify:

```bash
docker ps
```

---

# 🌐 Access the Application

Open your browser:

```
http://localhost:8080
```

If running on a remote server:

```
http://<Server-IP>:8080
```

---

# 📦 Docker Commands

## Build

```bash
docker build -t tic-tac-toe:v1 .
```

## Run

```bash
docker run -d --name tic-game -p 8080:80 tic-tac-toe:v1
```

## Stop

```bash
docker stop tic-game
```

## Start

```bash
docker start tic-game
```

## Restart

```bash
docker restart tic-game
```

## Remove Container

```bash
docker rm -f tic-game
```

## Remove Image

```bash
docker rmi tic-tac-toe:v1
```

---

# 🎮 How to Play

1. Open the application in your browser.
2. Player X starts the game.
3. Click an empty cell to place your mark.
4. Players alternate turns.
5. The first player to align three marks horizontally, vertically, or diagonally wins.
6. If all cells are filled without a winner, the game ends in a draw.
7. Click **Reset** to start a new game.

---

# 🔍 Application Workflow

```
User
   │
   ▼
Browser
   │
   ▼
Nginx Web Server
   │
   ▼
HTML
 │
 ├── CSS
 └── JavaScript
        │
        ▼
 Game Logic
```

---

# 📸 Screenshots

Add screenshots here.

Example:

```
screenshots/

home.png

winner.png

draw.png
```

---

# 📈 Future Enhancements

- Single-player mode (AI)
- Scoreboard
- Responsive mobile design
- Dark mode
- Sound effects
- Online multiplayer
- Player names
- Game timer

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch.

```bash
git checkout -b feature-name
```

3. Commit your changes.

```bash
git commit -m "Added new feature"
```

4. Push the changes.

```bash
git push origin feature-name
```

5. Create a Pull Request.

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Sravan Reddy**

Senior DevOps Engineer

---

# ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.
