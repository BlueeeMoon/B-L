# Capítulo 2

## Preguntas

### ¿Qué son las entradas y salidas de transacciones y qué tienen que ver con la transferencia de valor?

Las __UTXO__ (entradas y salidas de transacciones) representan la cantidad, monedas de Bitcoin en valor que se almacena en la cadena de bloques en una dirección de 
Bitcoin específica.

Cuando se dice que la billetera de un usuario ha recibido bitcoin, lo que queremos decir es que la billetera ha detectado una UTXO que se puede gastar con una de 
las claves controladas por esa billetera.

Los nodos completos de Bitcoin rastrean todas estás salidas disponibles y gastables y existe una base de datos denominada chainstate que contiene las UTXO y 
que se utiliza para evitar tener que realizar ciertas búsquedas sobre toda la cadena de bloques.

Así que las __UTXO__ son monedas en Bitcoin que se transfieren de un nodo a otro en toda la red como valor. 

Satoshi Nakamoto en el documento técnico: __Bitcoin: Un Sistema de Efectivo Electrónico Usuario-a-Usuario.__

> *Normalmente habrán o una sola entrada de una transacción previa más grande o múltiples entradas combinando cantidades más pequeñas, y al menos dos salidas: una para el pago, 
> y una para devolver el cambio, si es que hay algún cambio, de vuelta al emisor.*

### ¿Por qué se necesita una tarifa de transacción y cómo se calcula?



### ¿Por qué muchas transacciones de bitcoin incluirán una salida controlada por el remitente, además de la salida que paga al receptor? ¿Cuándo no ocurriría esto?

### ¿Qué es un pool de minería y por qué alguien pertenecería a uno?

### ¿Cuál es el estado de una transacción que aún no se ha incluido en un bloque, pero se ha propagado por la red? ¿Por qué algunos servicios requieren 6 confirmaciones para liquidar fondos?"

### ¿Qué tipo de privacidad existe para las transacciones en un libro mayor público?
