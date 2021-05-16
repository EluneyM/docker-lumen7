# Lumen 7

Docker con lumen 7 para proyectos de APIs, también incluye npm, artisan y composer para usar desde fuera del contenedor
usando el comando docker-compose run.

## Requerimientos

Se requiere la instalación de [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git), [docker](https://docs.docker.com/engine/install/) y [docker-compose](https://docs.docker.com/compose/install/).

## Instalación


1. Clonar el proyecto

    ```
    git clone https://github.com/EluneyM/docker-lumen7.git
    ```
    
2. Moverse a la raíz del proyecto

    ```
    cd docker-lumen7
    ```


3. Copiar archivo .env.example de la raíz del proyecto

    ```
    cp .env.example .env
    ```

4. Copiar archivo src/.env.example de la carpeta de Laravel

    ```
    cp src/.env.example src/.env
    ```

5. Editar las variables de entorno en el archivo de la raíz del proyecto, puedes usar el editor que gustes. Ej: vim

    ```
    vim .env
    ```

6. Copiar el archivo docker-compose.dist.yml

    ```
    cp docker-compose.dist.yml docker-compose.yml
    ```

7. Editar el puerto si entra en conflicto con otros contenedores

    ```
    vim docker-compose.yml
    ```

8. Reconstruir imagen

    ```
    docker-compose up -d --build
    ```



## Uso

* Para comprobar que este funcionando lumen dirigirse en el navegar al siguiente enlace.

    ```
    localhost:8004
    ```

* Detener contenedores (en la raiz del proyecto)

    ```
    docker-compose down
    ```

* Ejecutar contenedores

    ```
    docker-compose up
    ```
