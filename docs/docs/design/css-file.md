## Estilos personalizados

mkdocs nos ofrece modificar a gran medida el 'front-end' basico de nuestro sitio, como logos, colores y fuente de letras.

Hay mas apartados que se pueden modificar, en esta parte de la documentacion, hablaremos unicamente de estos puntos

## file.css

Vamos a crear un archivo `.css`, este lo estaremos colocando dentro de la carpeta `stylesheets` dentro de la carpeta del proyecto

```
mkdocs.yml
docs/
    index.md
    stylesheets/
        custom.css
```

En pimera instancia, en nuestro archivo `custom.css` recomendamos contar con dos colores principales definidas en la clase `:root`. Tambien podemos considerar sus colores `dark` y `light`, pero por el momento nos enfocaremos unicamente en dos colores principales

```css
:root {
  --primary: #ff9f1c;
  --secondary: #2ec4b6;
}
```

Para que puedan ser considerados, debemos elegir variables ya establecidas en `mkdocs` para que sean sobreescritas. Esto lo haremos sobre la misma clase `:root` simplemente que seleccionando todos los elementos que puedan existir.

```css
:root > * {
  --md-primary-fg-color: var(--primary);
  --md-typeset-a-color: var(--secondary);
  --md-accent-fg-color: var(--secondary);
}
```


Para que estos cambios puedan ser tomados en cuenta, debemos agregar la siguiente linea en el archivo `mkdocs.yml`

```yml
extra_css:
  - stylesheets/custom.css
```


---

<!-- ## Modo oscuro -->