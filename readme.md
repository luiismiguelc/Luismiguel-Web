# Mi Portafolio Personal - Coderhouse

¡Hola! Este repositorio contiene la versión final de mi portfolio personal como diseñador UX/UI, refactorizado de CSS tradicional a una arquitectura modular con SCSS para facilitar su mantenimiento y escalabilidad.

Sitio en vivo: https://luismiguel-web.vercel.app

Tecnologías usadas:
- HTML5 con marcado semántico
- CSS3 y SCSS con partials, variables, mixins y la regla @use
- Bootstrap 5
- AOS (Animate On Scroll)

Estructura de estilos en la carpeta scss:
- utilities: variables y mixins globales
- base: reseteo y tipografía
- layout: header, nav y footer
- components: botones y tarjetas
- main.scss: orquestador principal

Para compilar Sass localmente:
npx sass scss/main.scss styles/styles.css
