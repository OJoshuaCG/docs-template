## Template

Este es una plantilla que puedes utilizar para crear documentacion, ademas de incorporar Github Actions para el despliegue de tu proyecto.

Esta realizado con el paquete `mkdocs` de `python`, el cual nos permite desarrollar la documentacion con ayuda de archivos markdown (**.md**)

Ademas de apoyarse del paquete `mkdocs-material`, el cual tiene muchas caracteristicas para crear una documentacion atractiva y personalizable.


---

## Clonar repositorio

Puedes clonar el repositorio, crear tu entorno virual e instalar sus dependencias.

```sh
git clone https://github.com/OJoshuaCG/docs-template.git
cd docs-template
python -m venv venv
source ./venv/bin/activate
pip install -r requirements.txt
```

Despues de crear el entorno virtual, puedes continuar con la modificacion de los archivos dentro de la carpeta **docs**.
Para poder visualizar los cambios y como se visualizaran en produccion, deberas ejecutar el comando `mkdocs serve` dentro de la carpeta donde se encuentra la documentacion.

```sh
cd docs
mkdocs serve
```


---

## Crear desde 0

Si deseas crear el proyecto desde 0, puedes comenzar instalando los paquetes necesarios en tu entorno.
Para despues ejecutar el comando correspondiente para crear los archivos necesarios que nos ayudaran a crear la documentacion.

```sh
pip install mkdocs-material
mkdocs new <project-name>
cd <project-name>
```

Una vez creado, debemos configurar ahora el proyecto para que tome en cuenta los estilos de material.
Para ello, editaremos el archivo `mkdocs.yml`

```yml
theme:
  name: material
```

Despues de elegir el tema 'material', podemos pre-visualizar nuestro sitio:

```sh
mkdocs serve
```