<p align="center">
  <a href="https://github.com/DNadas98/freeoam-hiking-companion-app/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/DNadas98/freeoam-hiking-companion-app.svg?style=for-the-badge" alt="Contributors">
  </a>
  <a href="https://github.com/DNadas98/freeoam-hiking-companion-app/issues">
    <img src="https://img.shields.io/github/issues/DNadas98/freeoam-hiking-companion-app.svg?style=for-the-badge" alt="Issues">
  </a>
  <a href="https://github.com/DNadas98/freeoam-hiking-companion-app/blob/master/LICENSE">
    <img src="https://img.shields.io/github/license/DNadas98/freeoam-hiking-companion-app.svg?style=for-the-badge" alt="License">
  </a>
  <a href="https://linkedin.com/in/daniel-nadas">
    <img src="https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555" alt="LinkedIn">
  </a>
</p>

<br xmlns="http://www.w3.org/1999/html"/>
<div align="center">
  <a href="https://github.com/DNadas98/freeoam-hiking-companion-app">
    <img src="https://avatars.githubusercontent.com/u/125133206?v=4" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">FreeRoam Hiking Companion Application</h3>
  <p align="center">
    Created by <a href="https://github.com/DNadas98">DNadas98 (Dániel Nádas)</a>
    <br />
    <a href="https://github.com/DNadas98/freeoam-hiking-companion-app/issues">Report Bug</a>
    ·
    <a href="https://github.com/DNadas98/freeoam-hiking-companion-app/issues">Request Feature</a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#tech-stack">Tech Stack</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#deployment">Deployment</a></li>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#setup--run">Setup and run</a></li>
      </ul>
    </li>
    <li>
      <a href="#usage">Usage</a>
    </li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#images">Images</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

## About The Project

The FreeRoam Hiking Companion Application is a personal development project aimed at enhancing my skills in AngularJS and Java Spring Microservices, while merging my passion for hiking with technology. This application is designed to serve as a comprehensive hiking trip planner where users can explore various hiking-related points of interest such as peaks, summits, and trails. Users can access detailed information, download route GPX files, and personalize their experience by creating an account to favorite locations and upload their own trail data. This project is currently in the initial phases of development, designed with scalability in mind to continuously integrate additional features and new technologies. The aim is to create an extendable platform that not only supports my learning objectives but also enhances the hiking community's access to valuable content.

## Repositories
The architecture of the project leverages a microservices approach, incorporating several key components:
#### Angular Client
- The client application with a dynamic [Leaflet JS](https://leafletjs.com/)-based map system, that allows users to explore trails and summits on open-source maps.
- [freeroam-frontend-angular](https://github.com/DNadas98/freeroam-frontend-angular)
#### Keycloak Authorization Server:
- An open source authorization server utilized to handle secure user authentication via OpenID Connect, manage service-to-service communication through OAuth2, and provide a dashboard for efficient administration of users, roles, and permissions.
- [freeroam-keycloak](https://github.com/DNadas98/freeroam-keycloak)
#### Eureka Discovery Service:
- Manages service registration and discovery, enabling dynamic interaction between the microservices.
- [freeroam-eureka](https://github.com/DNadas98/freeroam-eureka)
#### Reactive Spring Gateway:
- Acts as an intelligent router that directs incoming API requests to the appropriate backend services, facilitating a responsive user experience.
- [freeroam-gateway](https://github.com/DNadas98/freeroam-gateway)
#### Summits Service:
- Collects and manages data related to summits and peaks, offering access to extensive geographical and hiking trail information.
- [freeroam-summits](https://github.com/DNadas98/freeroam-summits)
#### Trails Service:
- Focuses on managing trail routes, first the ones collected from open APIs, then later on in development also the user-uploaded ones.
- [freeram-trails](https://github.com/DNadas98/freeroam-trails)

## Tech Stack

### Frontend

[![Angular JS](https://img.shields.io/badge/-Angular_JS-C3002F?style=for-the-badge&logo=angular&logoColor=black)](https://angular.io/)  
[![Angular Material UI](https://img.shields.io/badge/-Angular_Material_UI-005CBB?style=for-the-badge&logo=materialui&logoColor=white)](https://material.angular.io/)  
[![Leaflet JS](https://img.shields.io/badge/-Leaflet_JS-FFD62D?style=for-the-badge)](https://leafletjs.com/)  

### Backend

[![Java](https://img.shields.io/badge/-Java-ED8B00?style=for-the-badge)](https://www.java.com/en/)  
[![Eureka Discovery Service](https://img.shields.io/badge/-Eureka_Discovery_Service-CCCCCC?style=for-the-badge)](https://github.com/Netflix/eureka)  
[![Keycloak](https://img.shields.io/badge/-Keycloak_Authorization_Server-008AAA?style=for-the-badge)](https://www.keycloak.org/)  
[![Spring Gateway](https://img.shields.io/badge/-Spring_Gateway-589133?style=for-the-badge&logo=spring&logoColor=black)](https://docs.spring.io/spring-cloud-gateway/reference/spring-cloud-gateway.html)  
[![Spring Security](https://img.shields.io/badge/-Spring_Security-589133?style=for-the-badge&logo=spring&logoColor=black)](https://spring.io/projects/spring-security)  
[![Spring OAuth2 Client and Resource Servers](https://img.shields.io/badge/-Spring_OAuth2-589133?style=for-the-badge&logo=spring&logoColor=black)](https://spring.io/guides/tutorials/spring-boot-oauth2)

### Database, ORM

[![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=black)](https://www.postgresql.org/)
[![Hibernate ORM](https://img.shields.io/badge/-Hibernate_ORM-CCCCCC?style=for-the-badge&logo=hibernate&logoColor=black)](https://hibernate.org/orm/)
[![Spring Data JPA](https://img.shields.io/badge/-Spring_Data_JPA-589133?style=for-the-badge&logo=spring&logoColor=black)](https://spring.io/projects/spring-data-jpa)

### Integration and Deployment

[![Docker](https://img.shields.io/badge/-Docker-1d63ed?style=for-the-badge&logo=docker&logoColor=black)](https://www.docker.com/)
[![GitHub Actions](https://img.shields.io/badge/-GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=black)](https://github.com/features/actions)
[![Nginx](https://img.shields.io/badge/-Nginx-227722?style=for-the-badge&logo=nginx&logoColor=black)](https://www.nginx.com/)

## Getting Started

### Deployment

WORK IN PROGRESS

### Prerequisites

WORK IN PROGRESS

### Setup & Run

WORK IN PROGRESS

## Usage

WORK IN PROGRESS

## Roadmap

- See the [open issues](https://github.com/DNadas98/freeoam-hiking-companion-app/issues) for a
  full list of proposed features (and known issues).

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Images

WORK IN PROGRESS

## Contact

Dániel Nádas

- My GitHub profile: [DNadas98](https://github.com/DNadas98)
- My webpage: [dnadas.net](https://dnadas.net)
- E-mail: [daniel.nadas@dnadas.net](mailto:daniel.nadas@dnadas.net)
- LinkedIn: [Dániel Nádas](https://www.linkedin.com/in/daniel-nadas)

Project
Link: [https://github.com/DNadas98/freeoam-hiking-companion-app](https://github.com/DNadas98/freeoam-hiking-companion-app)
