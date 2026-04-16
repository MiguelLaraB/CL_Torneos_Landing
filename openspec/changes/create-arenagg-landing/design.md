## Context

El objetivo de este proyecto es construir una "Landing Page" responsiva para la plataforma ficticia "ARENAGG" como parte del portafolio del desarrollador. El sistema actual ya cuenta con un archivo `astro.config.mjs`, lo que indica que se utilizará el framework de Astro para un sitio estático optimizado. Este diseño se enfoca en componentes de UI limpios y modulares para lograr el máximo rendimiento y una experiencia de usuario temática ("gamer").

## Goals / Non-Goals

**Goals:**
- Implementar una interfaz de usuario fiel al diseño visual proporcionado (paleta oscura, fuentes cyberpunk/modernas, diseño asimétrico/angular).
- Construcción modular usando componentes de Astro (`.astro`).
- Garantizar que el diseño sea *mobile-first* y completamente responsivo (usando CSS Flexbox y CSS Grid).

**Non-Goals:**
- No se implementarán integraciones reales con backend, bases de datos o servicios de autenticación de terceros. Es puramente visual (Demo frontend).

## Decisions

- **Framework**: Se utiliza Astro en su configuración estática por defecto para entregar HTML puro, maximizando el rendimiento (cargas ultrarrápidas). No se utilizarán frameworks complejos de estado como React o Vue a menos que sea estrictamente necesario para la interactividad específica de un componente complejo, y en su lugar se usarán simples scripts JS "Vanilla" en Astro o componentes funcionales de Astro para la maquetación.
- **Estilos**: Se emplearán módulos CSS o Vanilla CSS globales en lugar de TailwindCSS a menos que esté ya configurado (dado el requerimiento de usar CSS puro/flexible y los principios de la app moderna con Astro). La paleta requerirá variables CSS globales.
- **Estructura de Componentes**:
  - `Navbar.astro`
  - `Hero.astro`
  - `TournamentList.astro` (Sidebar de próximos torneos)
  - `Stats.astro`
  - `Footer.astro`

## Risks / Trade-offs

- **Risk**: Complejidad en los recortes diagonales y bordes asimétricos típicos del diseño gamer.
  - **Mitigation**: Uso de propiedades como `clip-path` u `holographic/gradient borders` en CSS moderno en lugar de depender de múltiples imágenes PNG cortadas.
- **Risk**: Carga lenta de la imagen "Hero" de alta resolución.
  - **Mitigation**: Uso del componente `<Image />` integrado en Astro para optimización automática (WebP/AVIF).
