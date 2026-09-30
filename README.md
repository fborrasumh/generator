# Generator

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21423189.svg)](https://doi.org/10.5281/zenodo.21423189)

**Aplicación:** https://fborrasumh.github.io/generator/

Genera una **asignatura completa a partir de tus fuentes**: apuntes, transparencias o artículos. Siete agentes proponen el programa, que ajustas tema a tema, y después desarrollan cada apartado con fórmulas y ejemplos, preparan tests comprobados, dibujan mapas conceptuales, redactan la ficha docente y reúnen una **bibliografía que existe de verdad**. Aplicación de un solo fichero (`index.html`), sin servidor.

## Novedades de la versión 2.0

- Recorrido guiado con el estilo de Forja: **Fuentes → Asignatura → Programa → Generación → Resultado**.
- **Bibliografía solo real.** En la versión 1, la IA escribía referencias sin comprobarlas. Ahora vienen de dos orígenes:
  - las citadas en tus fuentes, comprobando que el autor y el año aparecen en el texto;
  - trabajos de OpenAlex con DOI, seleccionados por pertinencia.

  Las asignaturas antiguas avisan de que su bibliografía no está verificada.
- **Cuadernos Jupyter (.ipynb) como fuente**: se usan las celdas de texto, el código y las salidas de texto; los gráficos se indican como «[gráfico]».
- **PDF y Word se leen de verdad**: la versión 1 los leía como texto plano. Las fuentes ilegibles guardadas por la versión 1 se quitan con un aviso.
- **Tests validados por código**: cuatro opciones distintas, una correcta que exista, sin «todas/ninguna de las anteriores». Se reparan o se descartan, se mezclan las opciones y se basan en el contenido completo del apartado.
- **Contenido escapado**: el HTML que llegue en el texto generado no se ejecuta.
- **Programa editable** y **prueba con un solo tema** antes de generar el resto. Generación tema a tema con pausa y opción de detener; lo terminado se guarda.
- **Resultado** con buscador, tests interactivos con explicación y edición o regeneración de cada tema con una indicación.
- **Exportación** a Word (con clave de respuestas), Markdown con fórmulas, **tests para Moodle (GIFT)**, PDF y JSON.
- **Ejemplos**: una asignatura de muestra que se ve sin clave y dos apuntes de prueba.
- La evaluación de la ficha docente se presenta como propuesta, para ajustarla a la normativa del centro.
- Fichero de 135 KB (antes 865 KB): la librería de Word se carga al exportar. Compatible con las asignaturas y la base de datos de la versión 1. La clave pasa a ser la compartida del catálogo (`ia_openai_key`).

## Los agentes

| Agente | Qué hace |
|---|---|
| Planificador | Propone los temas y sus apartados a partir de las fuentes |
| Guía docente | Objetivos, competencias, metodología y propuesta de evaluación |
| Desarrollador | Contenido de cada apartado, con fórmulas en LaTeX y ejemplos |
| Tests | Preguntas sobre el contenido del apartado, validadas por código |
| Mapas | Mapa conceptual de cada tema |
| Bibliografía | Referencias de las fuentes y de OpenAlex, nunca inventadas |

## Privacidad

Fuentes y asignaturas se guardan en IndexedDB del navegador. El texto viaja a OpenAI; las búsquedas bibliográficas, a OpenAlex. Revisa el material antes de usarlo en clase.

## Cómo citar

Borrás Rocher, F. (2026). *Generator* (versión 2.0.0) [Software]. Universidad Miguel Hernández de Elche. https://doi.org/10.5281/zenodo.21423189

El DOI es el de concepto: apunta siempre a la última versión. GitHub ofrece la cita en APA y BibTeX con el botón *Cite this repository*, a partir de `CITATION.cff`.

Forma parte del catálogo [Herramientas IA para la academia](https://fborrasumh.github.io/ia/).

## Licencia

MIT © 2026 Fernando Borrás Rocher · Universidad Miguel Hernández de Elche.
