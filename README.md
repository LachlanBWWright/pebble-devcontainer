# 🚀 Pebble Developer Tools in a Containerized Environment

This repository provides a **containerized** development setup for [Pebble](https://rebble.io/), enabling an isolated and portable environment for Pebble SDK development. It supports both **Docker Compose** and **VS Code Dev Containers**, making it easy to get started with minimal setup.

Happy coding! 🚀🎉

---

## ✅ Prerequisites

Before setting up the environment, ensure you have the following installed:

- [Docker](https://www.docker.com/) – Required to run containers
- [VS Code](https://code.visualstudio.com/) & [Dev Containers Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) (Optional) – For using Dev Containers
- [Git](https://git-scm.com/) – To clone the repository

---

## 🚀 1. Setting Up with Docker Compose (Recommended)

This method provides the easiest and most streamlined way to run the Pebble development environment. If you are on Windows, you should run these commands through a WSL terminal to allow the emulator to function.

### **Steps:**

1. **Clone the repository:**

   ```sh
   git clone https://github.com/FBarrCa/pebble-devcontainer.git
   cd pebble-devcontainer
   ```
2. **Start the container:**

   ```sh
   docker compose up -d
   ```
3. **Access the container shell:**

   ```sh
    docker exec -it pebble-sdk-container zsh
   ```
4. **Stop and remove the container when done:**

   ```sh
   docker compose down
   ```

---

## 🖥️ 2. Setting Up with VS Code Dev Containers

If you're using **VS Code**, you can leverage **Dev Containers** to automatically set up and launch the environment inside a container. On Windows, you should use [VS Code in WSL](https://code.visualstudio.com/blogs/2020/07/01/containers-wsl#_open-vs-code-in-wsl-2) to allow the emulator to function.

### **Steps:**

1. **Clone the repository:**

   ```sh
   git clone https://github.com/FBarrCa/pebble-devcontainer.git
   cd pebble-devcontainer
   ```
2. **Open VS Code and load the project folder.**
3. When prompted, **click "Reopen in Container"**.
4. Wait for the container to build and start—then you're ready to code!

---

## 🤝 Contributing

We welcome contributions! To contribute:

1. **Fork** the repository.
2. Create a **new branch** for your changes.
3. Make your improvements.
4. Submit a **Pull Request** for review.
