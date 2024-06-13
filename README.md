# Basic OAT authentification example with AdonisJS v6

## Description
This is a basic example of how to implement OAT authentification with AdonisJS v6. It includes a simple user model and a basic authentification controller.

## Features
- Register a new user
- Login a user
- Logout the current user
- Get user details

## Installation

1. Clone the repository
```bash
git clone git@github.com:MaximeMRF/adonisjs-oat-auth-tutorial.git
```

2. Install the dependencies
```bash
npm install
```

3. Create a new .env file
```bash
cp .env.example .env
```

4. Start the server
```bash
node ace serve
```

## Deploy to docker

1. Build the image
```bash
docker build -t oat-tutorial .
```

2. Run the container
```bash
docker run -d --env-file .env.prod -p 3333:3333 oat-tutorial:latest
```
Save the container id to access it

3. Run the migrations manually
```bash
docker exec -it <container_id> /bin/bash
# when you are inside the container
node ./bin/console.js migration:run --force
# then exit the container with ctrl + d
```

Now you can access the server on `http://localhost:3333` 🚀

## Steps explanation

[🇬🇧 Read the tutorial](https://medium.com/@maximemrf/authentication-with-adonisjs-v6-and-access-token-oat-6c8029827562)

[🇫🇷 Lire le tutoriel](https://medium.com/@maximemrf/authentification-avec-adonisjs-v6-et-access-token-oat-83c97387a39b)
