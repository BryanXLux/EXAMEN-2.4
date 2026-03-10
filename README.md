# EXAMEN-2.4
Despliegue de un Sistema LMS Moodle con GitHub/Docker en una Mac Pro 2019

## Descripción

Este proyecto tiene como objetivo desplegar un sistema **LMS Moodle** utilizando **Docker**, permitiendo que cualquier integrante del equipo pueda levantar el entorno de manera rápida y sencilla en su equipo.
El uso de contenedores facilita la instalación, configuración y portabilidad del sistema en diferentes equipos.

---

## INTEGRANTES DEL EQUIPO

* Bryan Josué Mendoza Rodríguez 
* Alisson Monsterrat Jimenez Pat 
* Manuel Jesús Tah Canché

---

## Tecnologías utilizadas

* Docker
* Docker Compose
* Moodle LMS
* MySQL / MariaDB
* Git

---

## Requisitos previos

Antes de ejecutar el proyecto, asegúrate de tener instalado:

* Docker
* Docker Compose
* Git

Y contar con los siguientes archivos al clonar el repositorio:
* Dockerfile
* docker-compose.yml
* .env

Para verificar la instalación de las herramientas:

```
docker --version
docker-compose version
git --version
```

---

## Clonar el repositorio

Primero ejecutamos el siguiente comando para clonar este mismo repositorio:

```
git clone https://github.com/BryanXLux/EXAMEN-2.4.git
cd EXAMEN-2.4
```

---

## Levantar el entorno

Para iniciar los contenedores de Moodle:

```
docker-compose up -d
```

Esto descargará las imágenes necesarias y levantará los contenedores.
Toca esperar a que termine

---

## Acceder a Moodle

Una vez iniciado el sistema, abre tu navegador y entra a:

```
http://localhost
```

o en su defecto:
```
http://localhost:8080
```

Ahí podrás completar la **configuración inicial de Moodle**.

---

## Reiniciar la instalación desde cero

Si necesitas reiniciar completamente el sistema:

```
docker compose down -v
```

Luego vuelve a levantar el entorno:

```
docker compose up -d
```

Esto eliminará los contenedores y volúmenes para permitir una instalación limpia.

---

## Estructura del proyecto

```
moodle-docker/
│
├── docker-compose.yml
├── Dockerfile
├── .gitignore
├── README.md
```

---

## Notas importantes

* docker compose stop -> Apaga el contenedor
* docker compose start -> Prende el contenedor

---

