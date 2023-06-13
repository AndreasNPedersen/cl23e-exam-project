# Zay eCommerce

This is a demo project for Containerization & Linux elective at [UCL University College](https://ucl.dk)

The frontend is based on the following template:

* https://github.com/mosaadaldeen/zay-shop

# Hvordan man opstarter projektet i Docker

Gå ind i Frontend mappen og kør:
docker build -t frontend .
Gå ind i Backend mappen og kør:
docker build -t backend .

Gå ud i hoved mappen og kør:
docker stack deploy -c docker-compose.yml vandcykel

## Frontend

There is a specific README.md file in the frontend project

## Backend

There is a specific README.md file in the backend project
