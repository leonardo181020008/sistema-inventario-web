# Sistema de Inventario Web

Sistema de inventario desarrollado como proyecto web.
Actualmente incluye el frontend con HTML, CSS y JavaScript puro,
pensado para integrarse posteriormente con un backend en Java + Spring Boot.

## Tecnologías
- HTML5
- CSS3
- JavaScript (ES6)
- Git & GitHub
- (Próximamente) Java + Spring Boot

## Estructura del proyecto

sistema-inventario-web/
frontend/
│
├── index.html                # Página principal
├──                 
├── 
│
├── assets/
│   ├── img/                  # Imágenes
│   ├── icons/                # Íconos (svg, png)
│   └── fonts/                # Fuentes personalizadas
│
├── css/
│   ├── base/
│   │   ├── reset.css         # Reset / normalize
│   │   ├── variables.css     # Colores, fuentes, tamaños
│   │   └── global.css        # Estilos generales
│   │
│   ├── components/
│   │   ├── buttons.css
│   │   ├── forms.css
│   │   ├── tables.css
│   │   └── navbar.css
│   │
│   ├── pages/
│   │   ├── login.css
│   │   └── 
│   │
│   └── main.css              # Importa todos los CSS
│
├── js/
│   ├── config/
│   │   └── apiConfig.js      # URL del backend (Spring)
│   │
│   ├── services/
│   │   ├── authService.js    # Llamadas fetch (login, auth)
│   │   ├── userService.js    # fetch a usuarios
│   │   └── productService.js
│   │
│   ├── utils/
│   │   ├── validators.js
│   │   ├── formatters.js
│   │   └── alerts.js
│   │
│   ├── components/
│   │   ├── navbar.js
│   │   ├── modal.js
│   │   └── table.js
│   │
│   ├── pages/
│   │   ├── login.js
│   │   └── 
│   │
│   └── main.js               # Punto de entrada JS
│
└── README.md

backend/
│
├── pom.xml
├── README.md
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── leonardo/
│   │   │           └── inventario/
│   │   │
│   │   │               ├── InventarioApplication.java
│   │   │
│   │   │               ├── config/
│   │   │               │   ├── CorsConfig.java
│   │   │               │   └── SecurityConfig.java  
│   │   │
│   │   │               ├── controller/
│   │   │               │   ├── AuthController.java
│   │   │               │   ├── UserController.java
│   │   │               │   └── ProductController.java
│   │   │
│   │   │               ├── service/
│   │   │               │   ├── AuthService.java
│   │   │               │   ├── UserService.java
│   │   │               │   └── ProductService.java
│   │   │
│   │   │               ├── repository/
│   │   │               │   ├── UserRepository.java
│   │   │               │   └── ProductRepository.java
│   │   │
│   │   │               ├── model/
│   │   │               │   ├── User.java
│   │   │               └── └── Product.java
│   │   │
│   │   │               ├── dto/
│   │   │               │   ├── LoginRequestDTO.java
│   │   │               │   └── ProductDTO.java
│   │   │
│   │   │               ├── exception/
│   │   │               │   ├── GlobalExceptionHandler.java
│   │   │               │   └── ResourceNotFoundException.java
│   │   │
│   │   │               └── util/
│   │   │                   └── ResponseUtil.java
│   │   │
│   │   └── resources/
│   │       ├── application.properties
│   │       ├── application-dev.properties
│   │       └── data.sql
│   │
│   └── test/
│       └── java/
│           └── com/
│               └── leonardo/
│                   └── inventario/
│
└── .gitignore