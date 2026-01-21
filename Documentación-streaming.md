<h1 align="center">Documentación Streaming</h1>
<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/servicios-de-streaming.png"></p>
<br>
<p><b>Nombre: </b>Israel Moreno Ballesta</p>
<p><b>Curso: </b>2ºASIR</p>
<p><b>Asignatura: </b>Servicios de Red e Internet</p>
<p><b>Fecha: </b> 12/01/2026</p>

# ÍNDICE

- [Introducción](#introducción)
- [Práctica: radio online](#práctica-radio-online)
- [Práctica vídeo](#práctica-vídeo)
- [Anexo](#anexo)

## Introducción

Servicios de streaming son sistemas que permiten transmitir audio y vídeo por Internet sin descargar el archivo completo. Funcionan enviando el contenido en tiempo real mediante protocolos especializados y servidores dedicados. Son esenciales para reproducir música, películas y emisiones en directo desde cualquier dispositivo, adaptándose a la velocidad de conexión del usuario.

## Práctica: radio online

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
<a name="inicio-pasos"></a>

Una vez tenemos instalada la aplicación, la ejecutamos, vamos a **Opciones → Preferencias** y en **Emisión en vivo** configuramos los parámetros necesarios tomando como referencia la imagen del anexo. [Ver imagen](#configuración-emisión-en-vivo)

Una vez hecho esto, le damos a aplicar y a aceptar, insertamos una música y le damos al botón que pone **ON AIR**. [Ver imagen](#emitir-en-vivo)

Esperamos a que el botón se ponga en verde que significará que ya estamos emitiendo y le damos al **Play** para que la música comience. [Ver imagen](#comprobación-emisión-en-vivo)

Ahora vamos a la máquina que hace de servidor, abrimos el navegador y escribimos la dirección correspondiente, que en mi caso es `192.168.1.58:8000/israel`. [Ver imagen](#comprobación-emisión-en-vivo)

## Práctica vídeo

## Anexo

### Configuración emisión en vivo

<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/configuracion-emision-en-vivo.png"></p>

[Volver arriba](#inicio-pasos)

### Emitir en vivo

<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/insertar-musica-iniciar-emision.png"></p>

[Volver arriba](#inicio-pasos)

### Comprobación emisión en vivo

<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/emision-iniciada-reproducir-musica.png"></p>

[Volver arriba](#inicio-pasos)

### Comprobación

<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/comprobacion.png"></p>

[Volver arriba](#inicio-pasos)
