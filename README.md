# 🏹 IANSEO Docker Setup

This repository provides a Docker Compose setup to run the IANSEO
scoring system locally on macOS, Linux, or Windows.
It spins up two containers:

- Apache + PHP for the IANSEO frontend
- MySQL (or MariaDB) for the database backend

# 🚀 Quick Start
1. Clone the repository
```bash
git clone https://github.com/<your-username>/ianseo-docker.git
cd ianseo-docker
```

2. Download IANSEO

    Download the latest IANSEO release for Linux/Mac from:
👉 https://www.ianseo.net/Releases.php

3. Extract the contents into the ./ianseo/ folder in this repository:
```
ianseo-docker/
│
├── docker-compose.yml
└── ianseo/
    ├── index.php
    ├── Common/
    ├── ...
```

4. ▶️ Run the containers

    Start the environment:
    
    `docker compose up -d`
    
    
    This will:
    
    - Build the PHP/Apache image
    
    - Start a MariaDB database
    
    - Mount the IANSEO app from your local folder


5. Open http://localhost/ianseo
 in your browser.