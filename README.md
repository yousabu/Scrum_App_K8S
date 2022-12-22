## Scrum Application

This is a simple implementation of a Scrum Board, a tool that helps visualize and manage work. Originally it was first created in Toyota automotive, but nowadays it's widely used in software development.

A Scrum Board is usually made of 3 columns - *TODO*, *InProgres*s & *Done*. In each column there are Post-it notes that represents task and their status.

As already stated this project is an implementation of such board and made of 3 separate Docker containers that holds:

- PostgreSQL database
- Java backend (Spring Boot)
- Angular frontend
- Kubernetes


![swagger-ui](https://github.com/techtter/scrum-board/blob/master/assets/swagger.png)


This app is also put in Docker container and its definition can be found
in a file *scrum-app/Dockerfile*.



#### scrum-ui (Frontend)

This is a real endpoint for a user where they can manipulate their
scrums and tasks. It consumes the REST API endpoints provided by
*scrum-app*.

It can be entered using link: **http://localhost:4200/**
