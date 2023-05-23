# Docker-php-template
Minimal docker and php setup for my projects

## Usage
Move your php project to the app directory to look like:
- app
    - src
    - tmp

Run
```bash
    docker compose run -d --build
```

The php app should be on port 8088, while your mysql db is on port 4306
