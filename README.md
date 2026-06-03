# StudyGo — Pitch Deck Interactivo

> El **Sistema Operativo académico de la tecnología**: centraliza el aprendizaje, el desarrollo de software y la colaboración ágil en un solo espacio unificado para estudiantes y docentes.

Presentación de producto (pitch deck) construida como una **única página HTML autónoma**, con navegación por diapositivas, estética premium en modo oscuro y un módulo interactivo de funcionalidades. No requiere instalación, servidor ni proceso de compilación: basta abrir el archivo en un navegador.

---

## ✨ Características

- **6 diapositivas navegables** con transiciones suaves (fade + scale).
- **Navegación múltiple**: botones de avance/retroceso, atajos de teclado e indicadores de página clicables.
- **Módulo de funcionalidades interactivo**: cuadrícula de 6 categorías que abren un *modal* con el detalle de cada herramienta.
- **Diseño responsive** con layouts de alta fidelidad (incluye un *mockup* de la interfaz del aula).
- **Cero dependencias locales**: todo se carga vía CDN.

### Contenido de las diapositivas

| # | Diapositiva | Descripción |
|---|-------------|-------------|
| 1 | **Portada / Hero** | Título, propuesta de valor y llamada a la acción. |
| 2 | **El Problema** | La fragmentación digital académica y sus métricas (70% del tiempo perdido en setups, 5+ apps por materia, pérdida de trazabilidad). |
| 3 | **La Solución** | El Hub Académico todo-en-uno, con un *mockup* del aula (asignaciones, tablero ágil, IDE y chat). |
| 4 | **Público Objetivo** | Los tres pilares: Estudiantes, Docentes y Administradores. |
| 5 | **Valor Diferencial y Futuro** | Impacto, escalabilidad y diferenciadores clave (feedback integrado, control de evidencias, OAuth unificado). |
| 6 | **Funcionalidades del Sistema** | Cuadrícula interactiva de 6 categorías con detalle en *modal*. |

### Categorías del módulo interactivo (Diapositiva 6)

- 💻 **Área de Trabajo** — IDE en navegador, entrega de proyectos, feedback y seguimiento de código.
- 🧑‍🏫 **Aulas Digitales** — gestión de usuarios y roles, tareas, calendario académico y dashboards.
- 📂 **Archivos y Nube** — organización inteligente, integración con Google Drive y almacenamiento de evidencias.
- 💬 **Comunicación** — chat interno, alertas en tiempo real y diálogo directo docente–alumno.
- 🛡️ **Accesos Seguros** — login con Google y GitHub vía OAuth, y control de permisos.
- 📊 **Métricas y Notas** — boletines automáticos, estadísticas de clase y monitoreo individual.

---

## 🛠️ Tecnologías

- **HTML5** — estructura de un solo archivo.
- **[Tailwind CSS](https://tailwindcss.com/)** (vía CDN) — estilos utilitarios y configuración de tema personalizada.
- **JavaScript (vanilla)** — navegación entre diapositivas y lógica del *modal*; sin frameworks.
- **[Google Fonts](https://fonts.google.com/)** — `Urbanist` (títulos) e `Inter` (cuerpo).
- **[Font Awesome 6.5.1](https://fontawesome.com/)** (vía CDN) — iconografía.

> ⚠️ Al usar recursos por CDN, se necesita **conexión a internet** para que los estilos, fuentes e iconos se vean correctamente.

---

## 🚀 Uso

1. Descarga o clona el archivo `presentaci_n_interactiva_studygo.html`.
2. Ábrelo con doble clic en cualquier navegador moderno (Chrome, Edge, Firefox, Safari).

Eso es todo. Para presentar, usa el modo pantalla completa del navegador (normalmente **F11**).

### Atajos de teclado

| Tecla | Acción |
|-------|--------|
| `→` / `Espacio` | Diapositiva siguiente |
| `←` | Diapositiva anterior |
| `Esc` | Cerrar el modal de funcionalidades |

También puedes navegar con los botones de flecha del pie de página o haciendo clic en los indicadores de página.

---

## 🎨 Personalización

Todo el contenido y los estilos viven dentro del mismo archivo HTML.

- **Colores y tema**: edita el bloque `tailwind.config` en el `<head>`. La paleta principal usa `brand.blue` (`#5e6ad2`), `brand.mint` (`#4ade80`) y los fondos oscuros `dark.bg` / `dark.card`.
- **Texto de las diapositivas**: cada diapositiva es un `<div id="slide-N">` dentro del `<main>`; modifica el contenido directamente.
- **Datos del módulo interactivo**: edita el objeto `featureData` en el `<script>` final para cambiar títulos, iconos o el listado de cada categoría.
- **Número de diapositivas**: si agregas o quitas diapositivas, actualiza la constante `totalSlides` y añade/elimina el indicador correspondiente en `#slide-indicators`.

---

## 📁 Estructura del proyecto

```
.
└── presentaci_n_interactiva_studygo.html   # Pitch deck completo (HTML + CSS + JS)
```

---

## 📄 Licencia

Define aquí la licencia del proyecto (por ejemplo, MIT) o las condiciones de uso interno que apliquen.
