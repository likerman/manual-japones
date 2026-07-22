# Guía de actualización del manual

Esta guía define el procedimiento para incorporar cada nueva clase sin perder consistencia entre el registro cronológico, los capítulos temáticos y el glosario.

## Principios editoriales

1. Toda palabra u oración debe incluir japonés, romaji y traducción al español.
2. No se deben introducir estructuras todavía no estudiadas en ejercicios básicos, salvo que estén marcadas como contenido adicional.
3. La forma en kana debe conservarse incluso cuando se agregue el kanji.
4. El romaji utiliza macrones para vocales largas cuando corresponde: `ō`, `ū`.
5. Las dudas no resueltas deben quedar marcadas; no se completan por conjetura.

## Incorporación de una clase

1. Copiar `plantillas/nueva-clase.qmd` y renombrarla como `AAAA-MM-DD.qmd`.
2. Registrar los temas trabajados y los ejemplos efectivamente vistos.
3. Agregar las palabras nuevas a `datos/vocabulario.csv`.
4. Trasladar la gramática y la escritura a sus capítulos temáticos.
5. Actualizar `08-registro-clases/indice.qmd`.
6. Agregar ejercicios de repaso y sus respuestas.
7. Renderizar la edición web para detectar enlaces o tablas rotas.

## Campos del glosario

- `japones`: forma principal en kanji o katakana; puede coincidir con kana.
- `kana`: lectura completa en hiragana o katakana.
- `romaji`: transliteración utilizada en el manual.
- `espanol`: traducción breve de consulta.
- `categoria`: grupo temático normalizado.
- `clase`: fecha de incorporación en formato `AAAA-MM-DD`.
- `notas`: pronunciación, consonantes dobles, vocales largas o uso especial.

## Flujo recomendado en GitHub

1. Crear una rama para la nueva clase.
2. Realizar los cambios de contenido.
3. Abrir un pull request con un resumen de lo incorporado.
4. Revisar escritura japonesa, romaji y traducciones.
5. Fusionar mediante *squash* para mantener un historial claro.
