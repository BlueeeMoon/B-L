
## ¿Cuál es la relación entre las claves privadas, las firmas y los testigos?

Bitcoin utiliza criptografía de clave pública  para controlar la propiedad de los fondos en forma de __claves digitales, direcciones y firmas digitales.__ 

De tal manera que cuando alguien quiere probar la autenticidad de datos utiliza una __huella digital__, que es simplemente un __hash criptográfico__ y cuando alguien quiere revelar el conocimiento de un secreto sin revelarlo utiliza una __firma digital__, que es como una firma manuscrita donde firmas para autorizar algo, sin embargo en Bitcoin la __firma digital__ está vinculada a un número aleatorio llamado clave privada no a la persona en sí. 

Así que tenemos estos datos:

- Las claves digitales son creadas por los usuarios en la billetera y son independientes al protocolo de Bitcoin, es decir; son administradas por la billetera, estas claves digitales son la clave pública y la clave privada.
- La clave pública deriva de la clave privada, la primera es utilizada para recibir los fondos y la segunda es para firmar; firma digital, que veremos en el siguiente párrafo.  
- La firma digital es la que autoriza que se pueden gastar los fondos, conocida también como testigo y se genera con la clave privada, así que el que tenga una copia de esta clave privada tendrá el control sobre el Bitcoin vinculado a ella. 
- La clave pública del destinatario está representada por su huella digital, llamada __dirección de Bitcoin__ que es la parte que puedes compartir para recibir los fondos. 

Así que cuando alguien comparte una dirección de Bitcoin lo que sucede es que a partir de la clave pública se generó esta dirección. 

## La clave pública está representada por una dirección. ¿Por qué necesitamos direcciones y no enviamos Bitcoin a las claves públicas?

Bitcoin utiliza criptografía asimétrica, lo que significa que se generan dos claves: __una pública y una privada__, siendo la primera la responsable del cifrado y la segunda del descifrado.

> Para obtener una dirección de Bitcoin se genera un hash criptográfico unidireccional produciendo una huella digital __hash__, este hash es fácil de hacer en una dirección, sin embargo es imposible de hacer en la dirección inversa. 

Lo que significa que esta __dirección__ puede ser compartida al mundo con la seguridad de que nadie puede revertir la función y obtener la clave privada a partir de la clave pública, siendo esto la base de la seguridad de los fondos. 

## ¿Qué es una función criptográfica unidireccional y cómo la utilizamos para derivar claves públicas?

Una función criptográfica unidireccional produce una huella digital o __hash__ de una entrada de tamaño arbitrario, es decir; una entrada siempre producirá el mismo hash.
Una entrada puede ser cualquier dato, llamado pre-imagen que producirá una salida de longitud fija, llamada hash.

Como el ejemplo siguiente:


