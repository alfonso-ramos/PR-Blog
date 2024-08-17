---
title: 'Cómo Personalizar los Colores de los Puntos y Números en Listas con HTML y CSS'
description: 'Solución fácil y rápida para cambiar el color de puntos y números de listas en HTML y CSS.'
pubDate: 'Aug 17 2024'
heroImage: '/imagenListas.jpeg'
---

Las listas son elementos básicos en la creación de páginas web, ya que nos permiten organizar información de manera clara y estructurada. Sin embargo, a veces es necesario personalizar su apariencia para que se adapten mejor al diseño de nuestro sitio. En este artículo, te mostraré cómo cambiar los colores de los puntos en una lista desordenada (`<ul>`) y los números en una lista ordenada (`<ol>`) utilizando solo HTML y CSS.

## La Solución Simple

Aunque pueda parecer complicado al principio, personalizar los colores de los puntos y números en listas es muy sencillo gracias al pseudo-elemento `::marker`. Este pseudo-elemento nos permite aplicar estilos específicos a los marcadores de listas, ya sean puntos, números u otros símbolos.

### Ejemplo de Código

A continuación, te muestro el código necesario para implementar esta personalización:

### HTML

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Listas con Colores Personalizados</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h2>Lista Desordenada</h2>
    <ul class="custom-ul">
        <li>Elemento 1</li>
        <li>Elemento 2</li>
        <li>Elemento 3</li>
    </ul>

    <h2>Lista Ordenada</h2>
    <ol class="custom-ol">
        <li>Elemento A</li>
        <li>Elemento B</li>
        <li>Elemento C</li>
    </ol>
</body>
</html>
```

### CSS

```css
/* Cambia el color de los puntos en la lista desordenada */
.custom-ul {
    list-style-type: disc; /* Asegura que se utilicen puntos */
}

.custom-ul li::marker {
    color: blue; /* Cambia el color de los puntos */
}

/* Cambia el color de los números en la lista ordenada */
.custom-ol {
    list-style-type: decimal; /* Asegura que se utilicen números */
}

.custom-ol li::marker {
    color: red; /* Cambia el color de los números */
}
```

### Explicación del Código

- **Pseudo-elemento `::marker`:** Este pseudo-elemento se utiliza para seleccionar y aplicar estilos a los marcadores de las listas (`<ul>` y `<ol>`).
- **Personalización de los puntos en `<ul>`:** Con `.custom-ul li::marker { color: blue; }`, estamos asegurándonos de que los puntos de la lista desordenada sean de color azul.
- **Personalización de los números en `<ol>`:** Con `.custom-ol li::marker { color: red; }`, cambiamos el color de los números de la lista ordenada a rojo.

## Conclusión

Personalizar los colores de los puntos y números en listas con HTML y CSS es más fácil de lo que parece. Usando el pseudo-elemento `::marker`, puedes modificar la apariencia de las listas de manera sencilla, logrando que se adapten mejor al estilo de tu sitio web. ¡Espero que esta solución te haya sido útil!
