<h1 align="center">Documentación Streaming</h1>
<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/servicios-de-streaming.png" alt="servicios_streaming"></p>
<br>
<p><b>Nombre: </b>Israel Moreno Ballesta</p>
<p><b>Curso: </b>2ºASIR</p>
<p><b>Asignatura: </b>Servicios de Red e Internet</p>
<p><b>Fecha: </b> 12/01/2026</p>

# ÍNDICE

- [Introducción](#introduccion)
- [Práctica audio](#practica-audio)
  - [Radio online](#radio-online)
- [Práctica vídeo](#practica-video)

## Introducción

Servicios de streaming son sistemas que permiten transmitir audio y vídeo por Internet sin descargar el archivo completo. Funcionan enviando el contenido en tiempo real mediante protocolos especializados y servidores dedicados. Son esenciales para reproducir música, películas y emisiones en directo desde cualquier dispositivo, adaptándose a la velocidad de conexión del usuario.

## Práctica audio
### Radio online

Instalamos Icecast 2 en una máquina Ubuntu.

Primero haremos un update para que el sistema actualice la lista de paquetes disponibles, y después ejecutaremos el comando para instalar Icecast 2.

```bash
apt update
apt install icecast2
```
En otra máquina Ubuntu vamos a instalar la aplicación Mixxx.

Para ello primero añadimos los repositorios, después hacemos un update para que el sistema actualice la lista de paquetes disponibles, y después instalamos la aplicación.

```bash
add-apt-repository ppa:mixxx/mixxx
apt update
apt install mixxx
```

## Práctica vídeo
