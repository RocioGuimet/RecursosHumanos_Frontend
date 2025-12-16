# 🏢 Sistema de Gestión de Empleados - Frontend

Interfaz web moderna para gestionar empleados. Conecta con una API REST de Spring Boot para realizar operaciones CRUD completas con validación en tiempo real.

## 📸 Capturas de Pantalla

| Vista de Lista de Empleados | Agregar Empleado | Formulario de Edición |
| :---: | :---: | :---: |
| ![Vista Lista](https://raw.githubusercontent.com/RocioGuimet/RecursosHumanos_Frontend/main/Screenshots/Screenshot%20(1).png) | ![Vista Agregar](https://raw.githubusercontent.com/RocioGuimet/RecursosHumanos_Frontend/main/Screenshots/Screenshot%20(2).png) | ![Vista Formulario](https://raw.githubusercontent.com/RocioGuimet/RecursosHumanos_Frontend/main/Screenshots/Screenshot%20(3).png) |

## ✨ Lo que verás
- **Lista dinámica** de empleados con diseño responsive
- **Formularios inteligentes** con validación en tiempo real
- **Confirmaciones** antes de acciones críticas
- **Feedback inmediato** con mensajes de éxito y error

## 🚀 Tecnologías Utilizadas

* **Framework**: React 18 con Hooks
* **Enrutamiento**: React Router DOM para navegación entre vistas
* **Peticiones HTTP**: Axios para comunicación con la API REST
* **Estilos**: Bootstrap 5 para diseño responsive
* **Validación**: Implementación personalizada en tiempo real
* **Manejo de estado**: useState y useEffect para gestión de estado local

## 📦 Instalación y Ejecución Local

Sigue estos pasos para ejecutar el proyecto.

### **Prerrequisitos**
- Backend ejecutándose (https://github.com/RocioGuimet/RecursosHumanos_Backend)
- [React.js y npm](https://es.react.dev/)

### **1. Clonar el Repositorio**
```bash
git clone https://github.com/RocioGuimet/RecursosHumanos_Frontend.git
cd RecursosHumanos_Frontend
```

### **2. Instalar e iniciar**
```bash
npm install
npm start
```
La aplicación se abrirá automáticamente en http://localhost:3000.

### **3. ¡Listo!**

Asegurate de que el backend esté corriendo en http://localhost:8080
Si es así, ya podes utilizarlo


## 🎨 Experiencia de usuario

- **Diseño responsive** Se adapta a móviles, tablets y ordenadores
- **Mensajes** de éxito, error y advertencia. Feedbacks claros
- **Validación en tiempo real** Campos requeridos, sueldo positivo, errores que desaparecen al corregir
- **Interfaz intuitiva** con Bootstrap 5

## 💡 Consejo

Prueba primero el backend con Postman para asegurarte de que la API funciona correctamente.

## ⚙️ Flujo de comunicación

1. Frontend (React) → Petición HTTP con Axios → Backend (Spring Boot)

2. Backend procesa la petición → Responde con JSON → Frontend actualiza la UI

3. Validación coordinada: Validación en frontend (experiencia de usuario) + validación en backend (seguridad de datos)

## 📁 Estructura del Proyecto
```
RecursosHumanos_Frontend/
├── public/
│   ├── index.html              # Plantilla HTML principal
│   └── ...                     # Iconos y assets públicos
├── src/
│   ├── empleados/              # Componentes principales de empleados
│   │   ├── ListadoEmpleados.js # Lista principal
│   │   ├── AgregarEmpleado.js  # Formulario de creación
│   │   └── EditarEmpleado.js   # Formulario de edición
│   ├── plantilla/              # Plantilla
│   │   └── Navegacion.js       # Componente raíz con enrutamiento
│   ├── App.js                  # Función App
│   ├── App.css                 # Estilos principales
│   └── index.js                # Punto de entrada de React
├── Screenshots/                # Capturas para el README
├── package.json                # Dependencias y scripts de npm
└── README.md                   # Readme

