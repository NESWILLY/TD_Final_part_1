# TD Final Part 1: OpenAPI Specification for Football Competition Management API

This repository contains the OpenAPI specification for a web service that manages football competitions, teams, and players. The API allows for creating and retrieving competitions, teams, and players, with support for pagination and filtering.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Endpoints](#endpoints)
- [Schemas](#schemas)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project is part of the final assignment for the course "Introduction to Web Services (API)". The goal is to create an OpenAPI specification for a web service that manages football competitions, teams, and players.

## Features

- Create and retrieve competitions
- Create and retrieve teams
- Create, modify, and retrieve players for a specific team
- Pagination and filtering for list endpoints

## Endpoints

### Competitions

- **POST /competitions**: Create a new competition
- **GET /competitions**: Get a list of competitions with pagination

### Teams

- **POST /teams**: Create a new team
- **GET /teams**: Get a list of teams with pagination and filtering by team name

### Players

- **POST /teams/{teamId}/players**: Create a new player for a specific team
- **GET /teams/{teamId}/players**: Get a list of players for a specific team with pagination and filtering by player name

## Schemas

### Competition

- **name**: Name of the competition (e.g., LIGA)
- **location**: Country or continent where the competition takes place (e.g., SPAIN or EUROPE)

### Team

- **name**: Name of the team (e.g., Real Madrid)
- **slogan**: Slogan of the team (e.g., Hala Madrid)
- **competitions**: List of competitions the team participates in
- **players**: List of players in the team

### Player

- **name**: Name of the player (e.g., Cristiano Ronaldo)
- **number**: Player's number (e.g., 7)
- **strongFoot**: Player's strong foot (Left or Right)

## Usage

To use this OpenAPI specification, you can import the `openapi.yaml` file into any OpenAPI-compatible tool, such as Swagger UI or Postman.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have any suggestions or improvements.
