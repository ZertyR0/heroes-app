# 🦸‍♂️ Heroes App

**Aplicación web SPA desarrollada en Angular que permite la gestión completa de superhéroes con autenticación, CRUD operations, búsqueda inteligente y diseño responsivo.**

[![Angular](https://img.shields.io/badge/Angular-15.0.4-red)](https://angular.io/)
[![TypeScript](https://img.shields.io/badge/TypeScript-4.8.2-blue)](https://www.typescriptlang.org/)
[![Angular Material](https://img.shields.io/badge/Angular%20Material-15.1.0-indigo)](https://material.angular.io/)
[![JSON Server](https://img.shields.io/badge/JSON%20Server-0.17.1-green)](https://github.com/typicode/json-server)

## 📋 Descripción del Proyecto

Heroes App es una **Single Page Application (SPA)** moderna desarrollada con Angular 15 que implementa una arquitectura modular completa para la gestión de superhéroes. La aplicación incluye sistema de autenticación, operaciones CRUD completas, búsqueda con autocompletado en tiempo real y un diseño responsivo profesional.

### 🎯 Funcionalidades Principales

- ✅ **Sistema de Autenticación** - Login seguro con guards de protección
- ✅ **CRUD Completo** - Crear, leer, actualizar y eliminar héroes
- ✅ **Búsqueda Inteligente** - Autocompletado en tiempo real
- ✅ **Diseño Responsivo** - Adaptable a dispositivos móviles y desktop
- ✅ **Navegación Avanzada** - Rutas hijas y lazy loading
- ✅ **Material Design** - Interfaz moderna con Angular Material

## 🚀 Tecnologías Utilizadas

### Frontend
- **Angular**: 15.0.4
- **TypeScript**: 4.8.2
- **Angular Material**: 15.1.0
- **PrimeFlex**: 3.3.1
- **RxJS**: 7.5.0

### Backend Simulado
- **JSON Server**: 0.17.1
- **Node.js**: Para ejecutar JSON Server

### Herramientas de Desarrollo
- **Angular CLI**: 15.0.4
- **Karma**: 6.4.0 (Testing)
- **Jasmine**: 4.5.0 (Testing Framework)

## 📦 Instalación y Configuración

### Prerrequisitos
- Node.js 16 o superior
- npm o yarn
- Git

### 1. Clonar el Repositorio
```bash
git clone https://github.com/ZertyR0/heroes-app.git
cd heroes-app
```

### 2. Instalar Dependencias
```bash
npm install
```

### 3. Configurar Variables de Entorno
Las variables de entorno ya están configuradas:
- **Desarrollo**: `src/environments/environments.ts` → `http://localhost:3000`
- **Producción**: `src/environments/environments.prod.ts` → `https://geomaticanet.com/heroesApp`

## 🎮 Ejecución del Proyecto

### 1. Iniciar Backend (JSON Server)
```bash
# En una terminal
npm run backend
```
El backend estará disponible en: `http://localhost:3000`

### 2. Iniciar Frontend (Angular)
```bash
# En otra terminal
npm start
# o
ng serve
```
La aplicación estará disponible en: `http://localhost:4200`

### 3. Comandos Disponibles
```bash
# Desarrollo
npm start          # Iniciar aplicación Angular
npm run backend    # Iniciar JSON Server
npm run build      # Construir para producción
npm test           # Ejecutar pruebas unitarias

# Angular CLI
ng serve           # Servidor de desarrollo
ng build           # Construir proyecto
ng test            # Pruebas unitarias
ng generate        # Generar componentes/servicios
```

## 🗃️ Estructura del Proyecto

```
src/
├── app/
│   ├── auth/                 # Módulo de autenticación
│   │   ├── guards/          # Guards de protección
│   │   ├── pages/           # Páginas de login/registro
│   │   └── services/        # Servicios de autenticación
│   ├── heroes/              # Módulo principal de héroes
│   │   ├── components/      # Componentes reutilizables
│   │   ├── interfaces/      # Interfaces TypeScript
│   │   ├── pages/           # Páginas del módulo
│   │   ├── pipes/           # Pipes personalizados
│   │   └── services/        # Servicios de héroes
│   ├── material/            # Módulo Angular Material
│   └── shared/              # Componentes compartidos
├── assets/                  # Recursos estáticos
├── environments/            # Variables de entorno
└── data/                   # Base de datos JSON
```

## 🔐 Credenciales de Acceso

Para acceder a la aplicación, utiliza:
- **Email**: `andres.cruz@gmail.com`
- **Password**: Cualquier contraseña (simulación)

## 🌐 API Endpoints (JSON Server)

### Autenticación
- `GET /users` - Obtener usuarios

### Héroes
- `GET /heroes` - Listar todos los héroes
- `GET /heroes/:id` - Obtener héroe específico
- `POST /heroes` - Crear nuevo héroe
- `PATCH /heroes/:id` - Actualizar héroe
- `DELETE /heroes/:id` - Eliminar héroe
- `GET /heroes?q={query}&_limit=6` - Búsqueda con filtro

## 🏗️ Arquitectura y Patrones

### Características Técnicas
- **Lazy Loading**: Carga perezosa de módulos
- **Guards**: Protección de rutas con AuthGuard y PublicGuard  
- **Formularios Reactivos**: Validaciones con Angular Forms
- **Observables**: Programación reactiva con RxJS
- **Pipes Personalizados**: Transformación de datos (HeroImagePipe)
- **Material Design**: UI/UX consistente
- **TypeScript Estricto**: Tipado fuerte e interfaces

### Módulos Implementados
- **AuthModule**: Gestión de autenticación
- **HeroesModule**: CRUD de héroes
- **MaterialModule**: Componentes Angular Material
- **SharedModule**: Componentes reutilizables

## 📱 Responsive Design

La aplicación está optimizada para:
- 📱 **Móviles** (320px - 767px)
- 📊 **Tablets** (768px - 1023px)  
- 💻 **Desktop** (1024px+)

Utiliza **PrimeFlex** para el sistema de layout flexible y **Angular Material** para componentes adaptativos.

## 🧪 Testing

```bash
# Ejecutar pruebas unitarias
npm test

# Ejecutar pruebas en modo watch
ng test --watch

# Generar reporte de cobertura
ng test --code-coverage
```

## 📸 Capturas de Pantalla

### Dashboard Principal
![Heroes List](https://via.placeholder.com/800x400/1976D2/ffffff?text=Heroes+Dashboard)

### Sistema de Búsqueda
![Search Feature](https://via.placeholder.com/800x400/DC004E/ffffff?text=Search+%26+Autocomplete)

### Formulario de Héroes  
![Hero Form](https://via.placeholder.com/800x400/388E3C/ffffff?text=Hero+Form+CRUD)

## 🚀 Deploy y Producción

### Build para Producción
```bash
ng build --configuration production
```

### Variables de Entorno de Producción
El proyecto está configurado para usar `environments.prod.ts` en producción con la URL base: `https://geomaticanet.com/heroesApp`

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Para contribuir:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. Commit tus cambios (`git commit -m 'Agregar nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - mira el archivo [LICENSE](LICENSE) para más detalles.

## 👨‍💻 Créditos

**Desarrollado por:** Andres Cruz  
**Email:** andres.cruz@gmail.com  
**GitHub:** [@ZertyR0](https://github.com/ZertyR0)

### Agradecimientos
- **Angular Team** - Por el increíble framework
- **Material Design** - Por los componentes UI
- **JSON Server** - Por la simulación de API sencilla
- **Superhero Images** - Recursos visuales de DC Comics y Marvel Comics

---

⭐ **¡Si te gustó el proyecto, no olvides darle una estrella en GitHub!** ⭐
