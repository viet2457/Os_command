# OS Command Injection Challenges

This project contains a series of Command Injection challenges designed for educational purposes. It uses Docker Compose to spin up multiple levels of challenges, allowing you to practice and understand command injection vulnerabilities in a safe, isolated environment.

## Challenges

The project consists of 7 levels, each accessible on a different port:

| Level | Port | Description |
|-------|------|-------------|
| Level 01 | 3001 | Basic Command Injection |
| Level 02 | 3002 | Command Injection with filters |
| Level 03 | 3003 | Advanced filters |
| Level 04 | 3004 | Blind Command Injection |
| Level 05 | 3005 | Network restricted environment |
| Level 06 | 3006 | Read-only filesystem |
| Level 07 | 3007 | Complex environment |

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Installation & Usage

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd os_command_injection/command_injection
    ```

2.  **Start the challenges:**
    ```bash
    docker-compose up -d
    ```

3.  **Access the challenges:**
    Open your web browser and navigate to `http://localhost:<port>` corresponding to the level you want to try (e.g., `http://localhost:3001` for Level 1).

4.  **Stop the challenges:**
    ```bash
    docker-compose down
    ```

## Structure

- `cmdi_levelX/`: Contains the source code and Dockerfile for each level.
- `docker-compose.yml`: Orchestrates the containers and networking.

## Disclaimer

This project is for **educational purposes only**. Do not use the techniques learned here on systems you do not own or have explicit permission to test.
