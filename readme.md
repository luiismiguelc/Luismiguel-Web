# Portfolio Personal - Refactorización SCSS

Este proyecto es el portafolio profesional de **Luismiguel | UX/UI**, refactorizado utilizando una arquitectura modular en **SCSS**.

## Arquitectura SCSS
El proyecto sigue el patrón de arquitectura modular dividida en partials organizados en la carpeta `scss/`:

- **`utilities/`**: Archivos globales como `_variables.scss` y `_mixins.scss`.
- **`base/`**: Estilos base, reseteo CSS y reglas de tipografía (`_base.scss`, `_tipografia.scss`).
- **`layout/`**: Estilos de estructura como cabecera, navegación y pie de página (`_header.scss`, `_nav.scss`, `_footer.scss`).
- **`components/`**: Componentes reusables como botones y tarjetas (`_buttons.scss`, `_cards.scss`).
- **`main.scss`**: Orquestador principal que importa todos los parciales mediante la regla `@use`.

## Instrucciones de Compilación

### Requisitos
- Node.js instalado en el sistema.

### Compilar SCSS a CSS
Para compilar manualmente el archivo principal de SCSS a CSS ejecute:

```bash
npx sass scss/main.scss styles/styles.css
