# Control de Planta Láctea

Simulador interactivo del proceso de industrialización de la leche (7 etapas: recepción, enfriamiento, estandarización, pasteurización, homogeneización, envasado y distribución), pensado para una exposición grupal con participación en vivo del curso.

Trabajo Práctico — UTN FRBA (2026).

## Qué hace

- **Pantalla del profesor**: avanza etapas, genera fallas y desvíos, agrega sustancias a la línea (cada una con su análisis de riesgo real), y lanza rondas de preguntas a los alumnos presentes.
- **Pantalla del alumno**: registro de presencia contra el padrón del curso, responde preguntas técnicas sobre el proceso y recibe corrección automática.
- **Pantalla proyectada**: vista pública del estado de la línea para toda el aula.
- Motor de reglas propio que evalúa cada intervención (temperatura, pH, tiempo, sustancias, fallas) contra los parámetros reales del proceso de pasteurización HTST.

## Stack

HTML + JavaScript vanilla, sin dependencias externas. El estado se sincroniza entre dispositivos mediante `window.storage`, la API de almacenamiento compartido de los artifacts de Claude — sin backend propio.

## Uso

Es un archivo estático (`index.html`). Se puede abrir directamente o publicar en GitHub Pages para tener un link único que use todo el curso.
