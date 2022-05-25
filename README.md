# Raspb-Rubber
Convertir raspberry Pico en una Rubber Ducky (relativamente facil)
NO ME HAGO RESPONSABLE POR EL MAL USO QUE SE LE PUEDA DAR A ESTA INFORMACION.
SE TE PIDE QUE USES ESTE CONOCIMIENTO PARA EL BIEN Y APOYO DE LAS PERSONAS Y NO BENEFICIARSE ACOSTA DE LAS DEMAS PERSONAS.

-EL CONOCIMIENTO ES LIBRE-.
QUANTUM TECHNOLOGY.

LEER ANTES DE HACER CUALQUIER COSA.

Bueno aqui estan  los pasos necesarios para poder crear una Rubber-Ducky a partir de una RaspberryPico y los archivos contenidos dentro de este repositorio.
Como primer punto se agregaron varios archivos y se mencionara con el paso de las instrucciones la funcion de cada uno de ellos.


1. Como primer paso se descargaran todos los archivos contenidos en este repositorio el cual contiene varios archivos y 1 carpeta (adafruit_hid, adafruit-circuitpython-raspberry_pi_6.3.0, code.py, flash_nuke.uf2, payload.dd)

2. Se conectara la raspberry pico a la pc y se metera el archivoo llamado "adafruit-circuitpython-raspberry_pi_6.3.0" y esperamos a que se reinicie la conexion. (a dia de hoy ya existe una version mejorada del circuitpython pero lo probe y funciona mejor con esta version (6.3.0) eso le introduce una clase de sistema operaticvo a la rapberry para que pueda ser leida por la pc.

3. Se introducira dentro de la carpeta lib la carpeta llamada "adafruit_hid"  lo que hace esta carpeta es "engañar" a la pc indicando que el dispositivo conectado es un teclado, mouse etc.

4. Se introduciran dentro de la carpeta de origen "CIRCUITPY" los archivos code.py y payload.dd lo que hace el code es ejecutar el archivo payload.dd el archivo "payload.dd" es el encargado de ejecutar el script dentro de el va a estar codificado el Script que se ejecutara PRECAUCION con esta parte recordemos que el Script (payload.dd) al momento de pegarlo se ejecutara en tu pc asi que hacerlo con precaucion y bajo tu propia responsabilidad se recomienda que al momento de terminar de copiar desconectar inmediatamente la raspberry para que no termine la ejecucion.

5. Normalmente al conectar la Raspberry de nuevo se ejecuta el Script y te permite entrar en ella para poder modificar el payload.dd en caso de que no lo permita. se tiene que hacer todo el procedimiento en dado caso de querer cambiar el script

Para eso es el archivo llamado "Flash_nuke" antes de conectarla le dejaremos presionado el boton "BOOTSEL" y la conectaremos sin dejar de presionar eso hara que se eliminen todos los archivos de la Raspberry. para que se borre completamente y de forma correcta solo bastara con copiar el archivo "Flash_nuke" dentro de la raspberry y esperar a que vuelva a conectarse.
