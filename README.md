# CSSDiner
Felix Josue Lopez 2021-0116

# Resumen y definiciones de Selectores CSS

## ID Selectors
- `#fancy`: Selecciona el elemento con el id "fancy".
- `#fancy pickle`: Selecciona los elementos `<pickle>` dentro del elemento con id "fancy".

## Class Selectors
- `.small`: Selecciona todos los elementos con la clase "small".
- `orange.small`: Selecciona los elementos `<orange>` que tienen la clase "small".

## Descendant Selectors
- `bento orange.small`: Selecciona los elementos `<orange>` con la clase "small" que están dentro de un elemento `<bento>`.

## Grouping Selectors
- `bento, plate`: Selecciona todos los elementos `<bento>` y `<plate>`.

## Universal Selector
- `*`: Selecciona todos los elementos.

## Child Selectors
- `plate *`: Selecciona todos los elementos que son hijos de `<plate>`.
- `plate > apple`: Selecciona todos los elementos `<apple>` que son hijos directos de `<plate>`.

## Adjacent Sibling Selector
- `plate + apple`: Selecciona el elemento `<apple>` que es inmediatamente siguiente a un elemento `<plate>`.

## General Sibling Selector
- `bento ~ pickle`: Selecciona todos los elementos `<pickle>` que son hermanos de un elemento `<bento>`.

## Pseudo-classes
- `orange:first-child`: Selecciona el primer hijo `<orange>` de su padre.
- `plate > :only-child`: Selecciona el único hijo de `<plate>`.
- `.small:last-child`: Selecciona el último hijo con la clase "small" de su padre.
- `:nth-child(3)`: Selecciona el tercer hijo de su padre.
- `bento:nth-last-child(3)`: Selecciona el tercer hijo desde el final dentro de un `<bento>`.
- `apple:first-of-type`: Selecciona el primer `<apple>` de su tipo en su contenedor.
- `:nth-of-type(even)`: Selecciona todos los elementos de su tipo en posiciones pares.
- `:nth-of-type(2n+3)`: Selecciona todos los elementos de su tipo en posiciones que cumplen con la fórmula 2n+3.
- `apple:only-of-type`: Selecciona el único `<apple>` de su tipo en su contenedor.
- `.small:last-of-type`: Selecciona el último elemento de su tipo con la clase "small".
- `bento:empty`: Selecciona todos los elementos `<bento>` que no tienen hijos.
- `apple:not(.small)`: Selecciona todos los elementos `<apple>` que no tienen la clase "small".

## Attribute Selectors
- `[for]`: Selecciona todos los elementos con el atributo `for`.
- `plate[for]`: Selecciona todos los elementos `<plate>` con el atributo `for`.
- `[for="Vitaly"]`: Selecciona todos los elementos con el atributo `for` cuyo valor es "Vitaly".
- `[for^="Sa"]`: Selecciona todos los elementos con el atributo `for` que comienza con "Sa".
- `[for$="ato"]`: Selecciona todos los elementos con el atributo `for` que termina en "ato".
- `[for*="obb"]`: Selecciona todos los elementos con el atributo `for` que contiene "obb".
