<h1 align="center">Documentación Streaming</h1>
<p align="center"><img src="img/servicios-de-streaming.png"></p>
<br>
<p><b>Nombre: </b>Israel Moreno Ballesta</p>
<p><b>Curso: </b>2ºASIR</p>
<p><b>Asignatura: </b>Servicios de Red e Internet</p>
<p><b>Fecha: </b> 21/01/2026</p>

# ÍNDICE

- [Introducción](#introducción)
- [Práctica: radio online](#práctica-radio-online)
- [Práctica vídeo](#práctica-vídeo)
- [Anexo](#anexo)

## Introducción

Servicios de streaming son sistemas que permiten transmitir audio y vídeo por Internet sin descargar el archivo completo. Funcionan enviando el contenido en tiempo real mediante protocolos especializados y servidores dedicados. Son esenciales para reproducir música, películas y emisiones en directo desde cualquier dispositivo, adaptándose a la velocidad de conexión del usuario.

## Práctica: radio online

Instalamos Icecast 2 en una máquina Ubuntu que hará de servidor.

Primero haremos un update para que el sistema actualice la lista de paquetes disponibles, y después ejecutaremos el comando para instalar Icecast 2.

```
apt update
apt install icecast2
```
En otra máquina Ubuntu vamos a instalar la aplicación Mixxx.

Para ello primero añadimos los repositorios, después hacemos un update para que el sistema actualice la lista de paquetes disponibles, y después instalamos la aplicación.

```
add-apt-repository ppa:mixxx/mixxx
apt update
apt install mixxx
```

<a name="paso-1"></a>
Una vez tenemos instalada la aplicación, la ejecutamos, vamos a **Opciones → Preferencias** y en **Emisión en vivo** configuramos los parámetros necesarios tomando como referencia la imagen del anexo. [Ver imagen](#configuración-emisión-en-vivo)

<a name="paso-2"></a>
Una vez hecho esto, le damos a aplicar y a aceptar, insertamos una música y le damos al botón que pone **ON AIR**. [Ver imagen](#emitir-en-vivo)

<a name="paso-3"></a>
Esperamos a que el botón **ON AIR** se ponga en verde que significará que ya estamos emitiendo y le damos al **Play** para que la música comience. [Ver imagen](#comprobación-emisión-en-vivo)

<a name="paso-4"></a>
Ahora vamos a la máquina que hace de servidor, abrimos el navegador y escribimos la dirección correspondiente, que en mi caso es `192.168.1.58:8000/israel`, para comprobar que la emisión se está realizando correctamente. [Ver imagen](#comprobación-desde-el-navegador)

<a name="paso-5"></a>
Y ahora vamos a hacerlo desde la aplicación VLC.

Instalamos la aplicación.

```
apt install vlc
```

Una vez instalada, abrimos la aplicación, vamos a **Medio → Abrir ubicación de red** ponemos la dirección `http://192.168.1.58:8000/israel` y le damos a reproducir. [Ver imágenes](#comprobación-desde-vlc)

<a name="paso-6"></a>

Ahora vamos a acceder a la radio de un compañero tanto desde el navegador como desde VLC. [Ver imágenes](#acceso-a-un-compañero)

## Práctica vídeo

## Anexo

### Configuración emisión en vivo

<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/configuracion-emision-en-vivo.png"></p>

[Volver](#paso-1)

### Emitir en vivo

<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/insertar-musica-iniciar-emision.png"></p>

[Volver](#paso-2)

### Comprobación emisión en vivo

<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/emision-iniciada-reproducir-musica.png"></p>

[Volver](#paso-3)

### Comprobación desde el navegador

<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/comprobacion-navegador.png"></p>

[Volver](#paso-4)

### Comprobación desde VLC

<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/conectar-en-vlc.png"></p>
<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/url-vlc.png"></p>
<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/comprobacion-vlc.png"></p>

[Volver](#paso-5)

### Acceso a un compañero

<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/.png"></p>
<p align="center"><img src="https://github.com/isrmorbal/SRI/blob/main/img/.png"></p>

[Volver](#paso-6)
