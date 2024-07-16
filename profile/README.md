# Soba AI

Welcome! Soba provides you with three main projects that work together to provide a solution for interacting with open-source LLM (Large Language Model) servers.

1. [Soba-Frontend](#soba-frontend)
2. [Soba-Server](#soba-server)
3. [Soba-Inferer](#soba-inferer)

## Quick Demo

<video src="https://github.com/user-attachments/assets/23eb3a4e-07c3-4691-9465-75c1705a5470" width="750" height="400" controls></video>

## Soba-Frontend

This `soba-frontend` project is built using React & Typescript to provide a responsive interface for interacting with a Local LLM server.

### Key Features:

- Developed with `React` and `Vite` using `Typescript`.
- Utilizes `React Router` for navigation.
- Supports Markdown rendering with `marked.js` and syntax highlighting with `highlight.js`.

### Installation Instructions:

1. **Install Node.js**: Ensure you have Node.js installed. You can download it from [Node.js official website](https://nodejs.org/).
2. **Clone the Repository**:
   ```bash
   git clone https://github.com/DoudouFanClub/soba-frontend.git
   cd soba-frontend
   ```
3. **Install Dependencies**:
   ```bash
   npm install
   ```
4. **Run the Development Server**:
   ```bash
   npm run dev
   ```

## Soba-Server

The `soba-server` project is developed in Golang to handle database operations, runtime data caching, and communication between the Frontend and LLM Inferer.

### Key Features:

- Developed using Golang.
- Uses `MongoDB` for database operations.
- Uses `Redis` for caching runtime data.

### Installation Instructions:

1. **Install WSL (Windows Subsystem for Linux)**: Follow the instructions on the [Microsoft WSL Documentation](https://docs.microsoft.com/en-us/windows/wsl/install).
2. **Install MongoDB**: Refer to the [MongoDB installation guide](https://docs.mongodb.com/manual/installation/) for your specific operating system.
3. **Install Redis**: Follow the installation instructions from the [Redis official documentation](https://redis.io/download).
4. **Clone the Repository**:
   ```bash
   git clone https://github.com/DoudouFanClub/soba-server.git
   cd soba-server
   ```
5. **Install Golang**: Download and install Go from the [official website](https://golang.org/dl/).
6. **Install Dependencies**:
   ```bash
   go mod tidy
   ```
7. **Run the Server**:
   ```bash
   go run .
   ```

## Soba-Inferer

This project connects open-source LLM models with the frontend, enabling users to interact with the models directly.

### Key Features:

- Developed using Python to integrate with LLM models.
- Uses `ollama` for model management.
- Uses `asyncio` for asynchronous operations.

### Installation Instructions:

1. **Install Python**: Ensure you have Python installed. You can download it from the [Python official website](https://www.python.org/).
2. **Clone the Repository**:
   ```bash
   git clone https://github.com/DoudouFanClub/soba-inferer.git
   cd soba-inferer
   ```
3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the Inferer**:
   ```bash
   python main.py
   ```
