# Manual de japonés

Manual personal y progresivo de estudio, construido a partir de las clases y consultas de Jeremías Likerman.

## Objetivo

Organizar en un único material de consulta:

- escritura japonesa;
- gramática;
- vocabulario;
- números, precios y horas;
- modelos de oración;
- ejercicios y respuestas;
- registro cronológico de las clases.

Cada entrada en japonés debe incluir, siempre que corresponda:

1. escritura japonesa;
2. romaji;
3. traducción al español.

## Tecnología

El proyecto utiliza [Quarto](https://quarto.org/) para generar:

- un libro web navegable;
- un PDF imprimible mediante LuaLaTeX;
- un glosario estructurado en CSV.

## Estructura de actualización

- `datos/vocabulario.csv`: fuente estructurada del glosario.
- `plantillas/nueva-clase.qmd`: ficha reutilizable para registrar una clase.
- `GUIA_ACTUALIZACION.md`: procedimiento editorial y técnico.
- `08-registro-clases/indice.qmd`: cronología general.

## Compilación local

Para previsualizar la edición web:

```bash
quarto preview
```

Para generar solamente la web:

```bash
quarto render --to html
```

Para generar el PDF se necesita LuaLaTeX y una fuente japonesa compatible:

```bash
quarto render --to pdf
```

## Automatizaciones

- `validar.yml`: comprueba la edición HTML en los pull requests.
- `publicar.yml`: publica la edición web en la rama `gh-pages`.
- `generar-pdf.yml`: genera el PDF por separado y lo guarda como artefacto de GitHub Actions.

## Estado

Versión de contenido en preparación: `v0.2`.
