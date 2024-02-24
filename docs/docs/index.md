# Template docs

Este es el archivo `index.md`, el cual podras modificar el inicio de tu pagina para dar una breve descripcion de tu proyecto o documentacion


---

## Arbol del proyecto

Puedes tener organizada tu documentacion por temas, tomando en cuenta cada folder como un tema en especifico

```
mkdocs.yml
docs/
    index.md
tema 1/
    index.md
    subtema.md
tema 2/
    index.md
```


---

## `mkdocs.yml`

A traves del archivo `mkdocs.yml` podemos definir nuestra navegacion, definir un nuevo archivo de estilo, tema, iconos, comportamiento, vista caracteristicas, plugins, extensiones y mas.

```yml
site_name: Docs Template
site_description: Plantilla para la documentacion

# Setting navigation titles and files
nav:
  - Primeros pasos: index.md
  - Diseño:
      - Archivo mkdocs.yml: design/mkdocs-yml.md
      - Archivo css: design/css-file.md
```

Puedes apoyarte del siguente [enlace](https://squidfunk.github.io/mkdocs-material/setup/) para descubrir la demas configuracion posible a cambiar.