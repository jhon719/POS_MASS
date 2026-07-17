<p align="center">
  <img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="320" alt="Laravel Logo">
</p>
<h1 align="center">POS MASS</h1>
 
<p align="center">
  Sistema de Punto de Venta (POS) construido con Laravel
</p>
<p align="center">
  <a href="http://mass.kodice.net.pe" target="_blank">
    <img src="https://img.shields.io/badge/🚀%20Ver%20Demo%20en%20Vivo-mass.kodice.net.pe-red?style=for-the-badge" alt="Demo en vivo">
  </a>
</p>
<p align="center">
  <b><a href="http://mass.kodice.net.pe" target="_blank">👉 http://mass.kodice.net.pe 👈</a></b><br>
  <sub>Proyecto desplegado y listo para usar</sub>
</p>
<p align="center">
  <a href="https://github.com/jhon719/POS_MASS"><img src="https://img.shields.io/badge/Repositorio-GitHub-181717?style=flat&logo=github" alt="Repositorio"></a>
  <img src="https://img.shields.io/badge/PHP-31.1%25-777BB4?logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/Blade-28.3%25-FF2D20?logo=laravel&logoColor=white" alt="Blade">
  <img src="https://img.shields.io/badge/License-MIT-green" alt="License">
</p>
---
 
## 📌 Enlaces rápidos
 
| Recurso | Enlace |
|---|---|
| 🌐 Demo desplegada | [http://mass.kodice.net.pe](http://mass.kodice.net.pe) |
| 💻 Repositorio | [github.com/jhon719/POS_MASS](https://github.com/jhon719/POS_MASS) |
 
---
 
## 📖 Concepto del proyecto
 
**POS MASS** es un sistema de **Punto de Venta (Point of Sale)** desarrollado sobre el framework **Laravel**. Está pensado para digitalizar y agilizar el proceso de ventas de un negocio: registro de productos, control de ventas, gestión de usuarios y generación de la información necesaria para la operación diaria de un comercio.
 
El proyecto sigue la arquitectura estándar de Laravel (MVC), utilizando **Blade** para las vistas y un flujo de assets moderno con **Vite**, lo que permite una interfaz ágil y mantenible.
 
> ℹ️ El repositorio no incluye una descripción oficial ampliada por parte del autor; el detalle funcional anterior se basa en el propósito general que indica el nombre del proyecto (POS) y su estructura de código. Se recomienda validar/ampliar esta sección con las funcionalidades específicas del negocio.
 
---
 
## 🛠️ Herramientas y tecnologías usadas
 
- **[Laravel](https://laravel.com)** — Framework backend en PHP (routing, ORM Eloquent, migraciones, etc.)
- **PHP** — Lenguaje principal del backend
- **Blade** — Motor de plantillas para las vistas
- **JavaScript** — Interactividad en el frontend
- **CSS** — Estilos de la interfaz
- **HTML** — Estructura de las vistas
- **[Vite](https://vitejs.dev)** (`vite.config.js`) — Compilación y bundling de assets
- **[Composer](https://getcomposer.org)** — Gestor de dependencias PHP
- **[NPM](https://www.npmjs.com)** — Gestor de dependencias JS
- **[Docker](https://www.docker.com)** (`Dockerfile`) — Contenerización del proyecto
- **[PHPUnit](https://phpunit.de)** (`phpunit.xml`) — Testing
- **GitHub Actions** (`.github/workflows`) — Integración continua (CI)
---
 
## 📂 Estructura del proyecto
 
```
POS_MASS/
├── .github/workflows/   # Workflows de CI/CD (GitHub Actions)
├── _source/             # Recursos/fuentes adicionales del proyecto
├── app/                 # Lógica de la aplicación (Modelos, Controladores, etc.)
├── bootstrap/           # Arranque del framework
├── config/              # Archivos de configuración de Laravel
├── database/            # Migraciones, seeders y factories
├── public/              # Punto de entrada público (index.php, assets compilados)
├── resources/           # Vistas Blade, CSS y JS sin compilar
├── routes/               # Definición de rutas (web.php, api.php, etc.)
├── storage/              # Archivos generados, logs, cache
├── tests/                 # Pruebas automatizadas
├── .env.example           # Plantilla de variables de entorno
├── artisan                 # CLI de Laravel
├── composer.json           # Dependencias PHP
├── package.json             # Dependencias JS
├── vite.config.js            # Configuración de Vite
├── Dockerfile                 # Imagen Docker del proyecto
└── README.md
```
 
---
 
## ⚙️ Requisitos previos
 
Antes de instalar el proyecto localmente, asegúrate de tener instalado:
 
- PHP >= 8.1
- [Composer](https://getcomposer.org)
- Node.js y NPM
- Una base de datos (MySQL, MariaDB, PostgreSQL, SQLite, etc.)
- (Opcional) Docker, si prefieres levantar el proyecto en contenedores
---
 
## 🚀 Instalación local
 
### 1. Clonar el repositorio
 
```bash
git clone https://github.com/jhon719/POS_MASS.git
cd POS_MASS
```
 
### 2. Instalar dependencias de PHP
 
```bash
composer install
```
 
### 3. Instalar dependencias de JavaScript
 
```bash
npm install
```
 
### 4. Configurar variables de entorno
 
```bash
cp .env.example .env
php artisan key:generate
```
 
Edita el archivo `.env` con los datos de conexión de tu base de datos y demás configuraciones necesarias.
 
### 5. Ejecutar migraciones (y seeders si aplica)
 
```bash
php artisan migrate
php artisan db:seed
```
 
### 6. Compilar los assets
 
```bash
npm run dev
```
 
### 7. Levantar el servidor local
 
```bash
php artisan serve
```
 
El proyecto quedará disponible en `http://127.0.0.1:8000`.
 
### (Alternativa) Ejecutar con Docker
 
```bash
docker build -t pos_mass .
docker run -p 8000:8000 pos_mass
```
 
---
 
## 🧪 Ejecutar pruebas
 
```bash
php artisan test
```
 
---
 
## 🤝 Contribuciones
 
Las contribuciones son bienvenidas. Si deseas colaborar:
 
1. Haz un fork del repositorio
2. Crea una rama para tu funcionalidad (`git checkout -b feature/nueva-funcionalidad`)
3. Realiza tus cambios y haz commit (`git commit -m 'Agrega nueva funcionalidad'`)
4. Sube tu rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request
---
 
## 📄 Licencia
 
Este proyecto está construido sobre el framework [Laravel](https://laravel.com), el cual es software de código abierto bajo la licencia [MIT](https://opensource.org/licenses/MIT).
