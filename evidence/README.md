# Evidencias de Desarrollo - Módulo de Cursos

Este documento resume las funcionalidades implementadas en el sistema de gestión de la escuela de conducción (Autoschool App) para el módulo de cursos.

## Funcionalidades Implementadas

### 1. Backend (Django REST Framework)
- **Modelado de Datos:** Definición de campos específicos para cursos (nombre, descripción, precio, duración y nivel) utilizando `DecimalField` para precisión en costos y `PositiveIntegerField` para horas.
- **API REST:** Implementación de endpoints siguiendo el patrón de diseño de Django mediante `ViewSets` y `Routers`, permitiendo el acceso estructurado a la información en `/api/courses/`.
- **Esquema de Documentación:** Configuración y verificación de la API a través de Swagger UI.

### 2. Frontend (Next.js & Shadcn/UI)
- **Listado Dinámico:** Renderizado de tablas interactivas para visualizar los cursos disponibles en tiempo real.
- **Formulario de Gestión:** Creación de un formulario robusto para el registro de nuevos cursos, integrando:
    - **Validación de Datos:** Uso de `Zod` y `React Hook Form` para asegurar la integridad de la información ingresada.
    - **Formateo de Moneda:** Implementación de lógica en TypeScript para mostrar precios con formato de moneda y decimales correctos (`.toFixed(2)`).
    - **Control de Niveles:** Selector personalizado para categorizar los cursos en niveles (Básico, Intermedio, Avanzado).

## Contenido de la Carpeta
- `swagger_endpoint.png`: Captura del endpoint funcionando en la documentación de la API.
- `listado_cursos.png`: Vista general del dashboard con los cursos de manejo registrados.
- `formulario_creacion.png`: Demostración de la interfaz para añadir o editar información.
