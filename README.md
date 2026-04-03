# 📊 Gestión de cualificación docente - UniCartagena

<div align="center">

[![Universidad de Cartagena](https://img.shields.io/badge/Universidad-Cartagena-blue?style=flat-square)](https://www.unicartagena.edu.co/)
[![Estado del Proyecto](https://img.shields.io/badge/Estado-Activo-green?style=flat-square)](https://github.com/Minogar28/TRABAJOS-U)
[![License](https://img.shields.io/badge/License-ISC-yellow?style=flat-square)](LICENSE)
[![JavaScript](https://img.shields.io/badge/JavaScript-94.5%25-yellow?style=flat-square)](https://developer.mozilla.org/es/docs/Web/JavaScript)

</div>

## 📌 Descripción del Proyecto

**GDocente** es una plataforma web integral desarrollada para la **Universidad de Cartagena** que permite la gestión completa de proyectos académicos, con enfoque especial en:

- 👨‍🏫 **Caracterización de Docentes** - Registro y gestión de información de profesores
- 🎓 **Gestión de Incentivos Académicos** - Administración de incentivos para docentes con seguimiento integral
- 📊 **Dashboard Administrativo** - Estadísticas y análisis en tiempo real
- 🔐 **Sistema de Autenticación Seguro** - Control de acceso basado en roles
- 📱 **Interfaz Responsiva** - Compatible con dispositivos móviles y desktop

---

## 🚀 Características Principales

### Gestión de Docentes
- ✅ Registro y actualización de información docente
- ✅ Búsqueda avanzada y filtros personalizados
- ✅ Descarga de reportes en Excel
- ✅ Validación de datos en tiempo real

### Gestión de Incentivos
- ✅ Creación y administración de incentivos académicos
- ✅ Seguimiento de incentivos (activos, vigentes, finalizados, eliminados)
- ✅ Sistema de reportes con validación en 3 estados (Validados, Pendientes, Rechazados)
- ✅ Estadísticas de distribución por tipo de incentivo
- ✅ Visualización de métricas en tiempo real

### Sistema de Autenticación
- ✅ Login seguro con JWT (JSON Web Tokens)
- ✅ Control de roles y permisos
- ✅ Encriptación de contraseñas (bcrypt)
- ✅ Sesiones con expiración de 2 horas

### Interfaz de Usuario
- ✅ Tema claro/oscuro personalizable
- ✅ Diseño moderno con Material-UI
- ✅ Panel de configuración de aspecto
- ✅ Navegación intuitiva y fluida

---

## 🛠️ Stack Tecnológico

### Frontend
- **React.js** - Librería para construcción de interfaces
- **Vite** - Herramienta de compilación rápida
- **Material-UI (MUI)** - Componentes de UI profesionales
- **React Router** - Enrutamiento de aplicación
- **Axios** - Cliente HTTP para API calls
- **Emotion** - Librería CSS-in-JS

### Backend
- **Node.js** - Runtime de JavaScript
- **Express.js** - Framework web minimalista
- **Sequelize** - ORM para gestión de bases de datos
- **PostgreSQL** - Base de datos relacional
- **JWT** - Autenticación con tokens
- **bcrypt** - Encriptación de contraseñas
- **Nodemailer** - Servicio de correo electrónico
- **Joi** - Validación de esquemas

### Herramientas Adicionales
- **XLSX** - Generación de reportes en Excel
- **Multer** - Gestión de carga de archivos
- **Cors** - Control de solicitudes entre dominios
- **Nodemon** - Reinicio automático durante desarrollo

---

## 📁 Estructura del Proyecto
TRABAJOS-U/
├── PROYECTOS_CUALIFICACION/ │
├── FRONTEND/ │
│
├── src/ │
│ │ ├── pages/ # Páginas principales 
│ │ │ │ ├── CaracterizacionDocentes/ 
│ │ │ │ └── gestionIncentivos/ 
│ │ │ ├── components/ # Componentes reutilizables 
│ │ │ ├── layouts/ # Layouts de la aplicación 
│ │ │ ├── states/ # Context API para estado global 
│ │ │ ├── theme/ # Configuración de temas 
│ │ │ ├── assets/ # Imágenes y estilos CSS 
│ │ │ ├── main.jsx # Punto de entrada 
│ │ │ └── App.jsx # Componente raíz 
│ │ ├── index.html 
│ │ ├── package.json 
│ │ └── vite.config.js 
│ │ │ ├── BACKEND/ 
│ │ ├── src/ 
│ │ │ ├── Models/ # Modelos Sequelize 
│ │ │ ├── Controllers/ # Lógica de negocios 
│ │ │ ├── Repositories/ # Acceso a datos 
│ │ │ ├── Routes/ # Definición de rutas 
│ │ │ ├── Middleware/ # Middlewares personalizados 
│ │ │ └── Utils/ # Funciones utilitarias 
│ │ ├── scripts/ # Scripts auxiliares 
│ │ ├── index.js # Punto de entrada 
│ │ ├── package.json 
│ │ └── constants.js 
│ │ │ ├── package.json 
│ └── .gitignore 
│ └── README.md



---

## 🔧 Instalación y Configuración

### Requisitos Previos
- Node.js (v14 o superior)
- npm o yarn
- PostgreSQL (v12 o superior)
- Git

### Pasos de Instalación

#### 1. Clonar el repositorio
git clone https://github.com/Minogar28/TRABAJOS-U.git
cd TRABAJOS-U/PROYECTOS_CUALIFICACION

#### 2. Instalación del Backend
cd BACKEND
npm install

###Crear archivo .env en la raíz del BACKEND:
# Base de Datos
DB_HOST=localhost
DB_PORT=5432
DB_NAME=trabajos_u
DB_USER=postgres
DB_PASSWORD=tu_contraseña

# JWT
TOKEN_SECRET=tu_clave_secreta_muy_segura

# Email
EMAIL_USER=tu_email@gmail.com
EMAIL_PASSWORD=tu_contraseña_app

# Puerto
PORT=5000

# Base de Datos
DB_HOST=localhost
DB_PORT=5432
DB_NAME=trabajos_u
DB_USER=postgres
DB_PASSWORD=tu_contraseña

# JWT
TOKEN_SECRET=tu_clave_secreta_muy_segura

# Email
EMAIL_USER=tu_email@gmail.com
EMAIL_PASSWORD=tu_contraseña_app

# Puerto
PORT=5000
Iniciar el Backend:

bash
npm start
# O en modo desarrollo con nodemon:
npm run dev
3. Instalación del Frontend
bash
cd ../FRONTEND
npm install
Crear archivo .env en la raíz del FRONTEND:

env
VITE_API_BASE_URL=http://localhost:5000/api
VITE_APP_NAME=TRABAJOS-U
Iniciar el Frontend:

bash
npm run dev
La aplicación estará disponible en: http://localhost:5173

📚 Guía de Uso
Acceso a la Aplicación
Login: Accede con tus credenciales de usuario
Dashboard: Visualiza estadísticas generales del sistema
Gestión de Docentes:
Busca, crea, edita y elimina docentes
Descarga reportes en Excel
Gestión de Incentivos:
Administra incentivos académicos
Revisa reportes y estadísticas
Valida reportes de docentes
Roles y Permisos
Rol	Descripción	Permisos
Admin	Administrador del sistema	Acceso completo a todas las funciones
Coordinador	Coordinador académico	Gestión de incentivos y reportes
Docente	Profesor universitario	Visualización de sus incentivos y reportes
Visualizador	Solo lectura	Acceso a reportes y estadísticas
🔐 Seguridad
Autenticación: JWT con expiración de 2 horas
Contraseñas: Encriptadas con bcrypt (10 rondas)
CORS: Configurado para solicitudes del frontend
Validación: Joi para validación de esquemas
Variables de Entorno: Uso de archivos .env para datos sensibles

📝 Notas Importantes
Asegúrate de configurar correctamente las variables de entorno antes de ejecutar la aplicación
La base de datos PostgreSQL debe estar en ejecución antes de iniciar el backend
El frontend requiere que el backend esté corriendo en http://localhost:5000
Los datos sensibles nunca deben ser compartidos o subidos al repositorio

<div align="center">
Desarrollado con ❤️ para la Universidad de Cartagena

⭐ Si este proyecto te fue útil, considera darle una estrella en GitHub

</div> 
