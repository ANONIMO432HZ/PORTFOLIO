# Portfolio Personal

Un portfolio web dinámico, responsivo y de alto rendimiento diseñado para destacar proyectos de desarrollo de software y ciberseguridad. Construido sobre **Astro**, cuenta con soporte multi-idioma nativo (i18n), tema oscuro persistente y un diseño visualmente premium con fondos de partículas y animaciones fluidas.

---

## 🚀 Inicio Rápido (Quick Path)

Para poner en marcha el proyecto localmente, sigue estos pasos:

1. **Instalar dependencias:**
   ```sh
   npm install
   ```
2. **Iniciar el servidor de desarrollo:**
   ```sh
   npm run dev
   ```
3. **Validar calidad de código y formatear:**
   ```sh
   npm run check
   ```
4. **Compilar para producción:**
   ```sh
   npm run build
   ```

---

## 🛠️ Stack Tecnológico & Arquitectura

El proyecto adopta un enfoque moderno enfocado en la velocidad de carga (Performance) y la simplicidad (Zero JS por defecto de Astro, hidratando solo lo necesario).

| Componente / Tecnología | Propósito |
| :--- | :--- |
| **Astro** | Generador de sitios estáticos ultrarrápido y flexible. |
| **TypeScript** | Programación segura para los scripts del cliente. |
| **Vanilla CSS** | Control total y modular del diseño sin sobrecarga de frameworks utilitarios. |
| **Biome** | Formateador y Linter unificado ultra veloz para el mantenimiento del estilo del código. |
| **AOS & Swiper** | Animaciones al hacer scroll y carruseles táctiles optimizados para móviles. |

---

## ✨ Características Principales

*   🌐 **Internacionalización (i18n):** Selector unificado en el Header que conmuta fluidamente entre Español (`es-ES`) e Inglés (`en-US`) de forma reactiva, leyendo traducciones de diccionarios JSON estructurados.
*   🌓 **Modo Oscuro Inteligente:** Implementación en el `Layout` con prevención de **FOUC** (Flash of Unstyled Content) leyendo de manera síncrona el `localStorage` antes de pintar la pantalla.
*   🌀 **Loader Spinner Centralizado:** Spinner de carga con transiciones suaves integrado en el core del layout global, asegurando una experiencia de transición premium en la carga inicial y recargas de cualquier página.
*   📦 **Estructura de Páginas Modular:**
    *   `/` (Home con secciones principales)
    *   `/about` (Detalles de perfil, trayectoria y habilidades)
    *   `/service` (Catálogo detallado de servicios y tarifas con acordeón FAQ interactivo)
    *   `/project` (Portafolio interactivo de proyectos organizado por categorías: aplicaciones y juegos)

---

## 📂 Estructura del Proyecto

```text
/
├── public/               # Assets públicos estáticos (imágenes de proyectos, favicon, etc.)
├── src/
│   ├── components/       # Componentes Astro reutilizables (Header, Footer, ParticleBackground, etc.)
│   ├── language/         # Diccionarios de traducción JSON (es.json y en.json)
│   ├── layouts/          # Layout.astro (plantilla principal que inyecta estilos, i18n, loader y modo oscuro)
│   ├── pages/            # Sistema de enrutamiento basado en archivos (.astro)
│   │   ├── index.astro   # Página principal
│   │   ├── about.astro   # Página sobre mí
│   │   ├── service.astro # Página de servicios
│   │   └── project/      # Subpáginas de proyectos (apps, juegos, index)
│   └── styles/           # Archivos CSS dedicados por páginas y componentes
├── biome.json            # Configuración de formateo y linting de Biome
├── tsconfig.json         # Configuración del compilador de TypeScript
└── astro.config.mjs      # Configuración general de Astro
```

---

## 🧞 Comandos de Consola

Todos los comandos se ejecutan desde la raíz del proyecto mediante tu terminal de preferencia:

| Comando | Acción |
| :--- | :--- |
| `npm run dev` | Inicia el servidor de desarrollo en `localhost:4321`. |
| `npm run build` | Compila el sitio estático optimizado en el directorio `./dist/`. |
| `npm run preview` | Previsualiza localmente la compilación de producción antes de desplegar. |
| `npm run format` | Aplica Biome para formatear de manera automática el código. |
| `npm run lint` | Ejecuta el linter de Biome para reportar malas prácticas. |
| `npm run check` | Analiza el código con Biome aplicando auto-fixes. |

---
*Desarrollado con pasión y buenas prácticas por Royer Valencia Arias.*
