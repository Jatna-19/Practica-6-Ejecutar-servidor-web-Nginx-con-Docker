# Práctica No. 6: Ejecutar un servidor web Nginx con Docker Compose

## Descripción

En esta práctica se creó y ejecutó un servidor web Nginx de forma local utilizando Docker Compose. El objetivo fue aprender a configurar un contenedor, compartir archivos HTML desde una carpeta local y comprobar el funcionamiento del servidor desde el navegador.

## Tecnologías utilizadas

- Docker Desktop
- Docker Compose
- Nginx
- HTML
- Git y GitHub

## Estructura del proyecto

```text
Practica-6-Ejecutar-servidor-web-Nginx-con-Docker/
├── src/
│   └── index.html
├── docker-compose.yml
└── README.md
```

## Configuración

El archivo `docker-compose.yml` utiliza la imagen de Nginx y configura el puerto 8080 de la computadora para acceder al puerto 80 del contenedor.

También se utiliza un volumen para conectar la carpeta `src` con el directorio `/usr/share/nginx/html` del contenedor, donde Nginx busca los archivos de la página web.

## Ejecución del proyecto

Para iniciar el servidor, se ejecuta el siguiente comando en la terminal, desde la carpeta principal del proyecto:

```bash
docker compose up -d
```

Para comprobar que el contenedor está funcionando:

```bash
docker compose ps
```

## Acceso al servidor

Con el contenedor en ejecución, se puede acceder a la página desde el navegador mediante la siguiente dirección:

http://localhost:8080

La página muestra el mensaje **Hola Mundo**, confirmando que el servidor web Nginx funciona correctamente.

## Conclusión

Con esta práctica aprendí a ejecutar un servidor web Nginx utilizando Docker Compose, configurar los puertos y montar una carpeta local como volumen. También comprobé que la página HTML se puede visualizar desde el navegador y que los archivos del proyecto pueden almacenarse en un repositorio de GitHub.

