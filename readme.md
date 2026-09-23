# Mi Portfolio Personal - Coderhouse

¡Hola! Este repositorio contiene la versión final de mi portfolio personal como diseñador UX/UI. Para esta entrega refactoricé todo el proyecto migrando de CSS tradicional a una arquitectura modular con **SCSS**, haciéndolo mucho más fácil de mantener y escalar.

## Arquitectura SCSS

Dividí los estilos en módulos pequeños dentro de la carpeta `scss/` para tener todo ordenado según la responsabilidad de cada archivo:

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
