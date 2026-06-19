# EspeLab — Sistema de Reservas de Laboratorios

## Descripción
EspeLab es un sistema web para la gestión y reserva de laboratorios académicos de la Universidad de las Fuerzas Armadas **ESPE**, sede Santo Domingo. Permite a los estudiantes y docentes consultar la disponibilidad de laboratorios y realizar reservas de forma digital.

## Objetivo
Digitalizar el proceso de reserva de laboratorios, eliminando conflictos de horario y facilitando el acceso a la información de disponibilidad en tiempo real.

## Tecnologías Utilizadas
- **HTML5** — Estructura semántica de las páginas
- **CSS3** — Estilos externos, Flexbox, CSS Grid, media queries, transiciones
- **Bootstrap 5.3** — Navbar, Carousel, Accordion, Modal, Alert, Badge, Progress Bar, Table
- **Font Awesome 6.5** — Íconos
- **Diseño Mobile-First** — Adaptable a móvil, tableta y escritorio

## Estructura de Carpetas

```
EspeLab/
│
├── index.html                  → Inicio de sesión
│
├── pages/
│   ├── Reserva/
│   │   └── Reserva.html        → Vista principal con todos los laboratorios
│   ├── Disponibles/
│   │   └── Disponibles.html    → Laboratorios disponibles
│   ├── Ocupados/
│   │   └── Ocupados.html       → Laboratorios ocupados
│   └── confirmacion/
│       └── confirmacion.html   → Confirmación de reserva
│
├── css/
│   ├── general.css             → Estilos compartidos (navbar, tarjetas, botones)
│   ├── index.css               → Login
│   ├── reserva.css             → Página principal de reservas
│   ├── disponibles.css         → Laboratorios disponibles
│   ├── ocupados.css            → Laboratorios ocupados
│   └── confirmacion.css        → Pantalla de confirmación
│
├── data/
│   ├── datos.json              → Estructura JSON de laboratorios y reservas
│   └── datos.xml               → Estructura XML de laboratorios y reservas
│
├── img/
│   ├── Logo.png
│   ├── Logo2.png
│   └── qr.png
│
├── icon/
│   ├── Computer_PC_Monitor_1906.ico
│   └── Logon_theapplication_2961.ico
│
└── README.md
```

## Páginas Disponibles

| Página | Descripción |
|---|---|
| `index.html` | Portal de autenticación (inicio de sesión) |
| `pages/Reserva/Reserva.html` | Vista principal: todos los laboratorios, carrusel, FAQ, modal de reserva |
| `pages/Disponibles/Disponibles.html` | Solo laboratorios disponibles |
| `pages/Ocupados/Ocupados.html` | Solo laboratorios ocupados + tabla de horarios |
| `pages/confirmacion/confirmacion.html` | Pase digital de confirmación con código QR |

## Componentes Bootstrap Utilizados

1. **Navbar** (`navbar`, `navbar-expand-lg`, `navbar-toggler`) — Menú de navegación responsive con colapso en móvil
2. **Carousel** (`carousel`, `carousel-item`, `carousel-fade`) — Carrusel de laboratorios destacados en la página de reservas
3. **Accordion** (`accordion`, `accordion-item`, `accordion-button`) — Sección de preguntas frecuentes
4. **Modal** (`modal`, `modal-dialog`, `modal-content`) — Formulario emergente para confirmar reserva
5. **Alert** (`alert`, `alert-success`, `alert-danger`, `alert-info`) — Mensajes informativos en cada página
6. **Badge** (`badge`, `bg-success`, `bg-danger`) — Etiquetas de estado en el carrusel
7. **Progress** (`progress`, `progress-bar`) — Barra de porcentaje de ocupación
8. **Table** (`tabla-horarios`) — Tabla de horarios reservados en página de ocupados

## Datos JSON y XML

Los archivos en la carpeta `data/` representan cómo se estructuraría la información del sistema si estuviera conectado a una base de datos o API:

- **`datos.json`** — Contiene la lista de laboratorios, sus datos (nombre, bloque, capacidad, estado, software), las reservas registradas y las estadísticas de ocupación.
- **`datos.xml`** — Misma información representada en formato XML con jerarquía de nodos.

En esta etapa los datos son simulados directamente en el HTML. En una implementación real, se obtendría esta información desde un servidor mediante `fetch()` o una API REST.

## Instrucciones para Ejecutar

1. Descarga o clona el repositorio.
2. Abre el archivo `index.html` en cualquier navegador moderno (Chrome, Firefox, Edge).
3. Navega a través de las páginas usando la interfaz.
4. No requiere servidor, base de datos ni instalación adicional.

## Autor

Erick Jardiel Maigua Toro
Proyecto final parcial 2 Fundamentos de sistemas web 