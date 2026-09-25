# Sistema de Gestión de Inventario (IMS)

![NodeJS](https://img.shields.io/badge/Node.js-v18%2B-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![ExpressJS](https://img.shields.io/badge/Express.js-4.x-000000?style=for-the-badge&logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15%2B-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![JavaScript](https://img.shields.io/badge/Vanilla_JS-ES6%2B-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

Plataforma integral de gestión de inventario orientada a la alta visibilidad, control de stock en tiempo real y trazabilidad operativa. El proyecto implementa una arquitectura desacoplada para garantizar escalabilidad, mantenibilidad y facilidad de despliegue.

---

## 🏗️ Arquitectura del Sistema

El proyecto está estructurado como un monolito desacoplado por servicios, facilitando la separación clara de responsabilidades:

```text
.
├── backend/            # API RESTful en Node.js + Express
│   ├── src/            # Lógica de negocio, controladores, rutas y modelos
│   ├── Dockerfile      # Configuración de Docker para el backend
│   └── package.json
├── frontend/           # Cliente SPA con Vanilla HTML5, CSS3 y JS Moderno (ES6+)
│   ├── public/         # Estilos, scripts y assets estáticos
│   ├── Dockerfile      # Nginx / Servidor estático para el cliente
│   └── index.html
├── docker-compose.yml  # Orquestador de contenedores (Backend, Frontend, PostgreSQL)
└── README.md