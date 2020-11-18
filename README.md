[![GitHub contributors](https://img.shields.io/github/contributors/HorebParraud/Popeye?style=for-the-badge)](https://github.com/HorebParraud/Popeye/graphs/contributors)
[![GitHub forks](https://img.shields.io/github/forks/HorebParraud/Popeye?style=for-the-badge)](https://github.com/HorebParraud/Popeye/network)
[![GitHub stars](https://img.shields.io/github/stars/HorebParraud/Popeye?style=for-the-badge)](https://github.com/HorebParraud/Popeye/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/HorebParraud/Popeye?style=for-the-badge)](https://github.com/HorebParraud/Popeye/issues)
[![GitHub license](https://img.shields.io/github/license/HorebParraud/Popeye?style=for-the-badge)](https://github.com/HorebParraud/Popeye)
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a>
    <img src="https://www.group-dis.com/wp-content/uploads/2017/11/devops-process.png" alt="Logo" width="500" >
  </a>

  <h1 align="center">Popey</h1>

  <p align="center">
    EPITECH project - DevOps
    <br />
    <br />
    <a href="https://github.com/HorepParraud/Popeye/issues">Report Bug</a>
    ·
    <a href="https://github.com/HorebParraud/Popeye/issues">Request Feature</a>
  </p>
</p>


<!-- IMPORTANT -->
## Important!
**If you are seeing this repository, please just ⭐ it! It will not take much time! :)**

<!-- ABOUT THE PROJECT -->
## About The Project
The goal of this project is to containerize and define the deployment of a simple web poll application

There are five elements constituting the application:

- **Poll**, a flask Python web application that gathers votes and push them into a `Redis` queue.

- **Redis**, which holds the votes sent by the Poll application, awaiting for them to be consumed by the `Worker`.

- **Worker**, a java application which consumes the votes being in the Redis queue, and stores them into a `PostgreSQL` database

- **PostgreSQL database**, which (persistently) stores the votes stored by the Worker.

- **Result**, a Node.js web application that fetches the votes from the database and displays the result

### Built With
* Docker-compose

<!-- GETTING STARTED -->
## Getting Started

Clone the repositorie and buil images with Docker-compose
```sh
docker-compose up --build
```
see Poll on `localhost:5000/` and Result on `localhost:5001/`

Do not forget to down containers
```sh
docker-compose down -v
```

<!--USEFULL LINKS-->
##
[![LinkedIn][linkedin-shield]][linkedin-url] [![GitHub][github-shield]][github-url]

<!-- MARKDOWN LINKS, ALIAS & IMAGES -->
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/horeb-parraud/
[github-shield]: https://img.shields.io/badge/-other_repositories-black.svg?style=for-the-badge&logo=github&colorB=555
[github-url]: https://github.com/HorebParraud?tab=repositories
