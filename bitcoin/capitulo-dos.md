# Capítulo 2

## Preguntas

### ¿Qué son las entradas y salidas de transacciones y qué tienen que ver con la transferencia de valor?

Las __UTXO__ (entradas y salidas de transacciones) representan la cantidad, monedas de Bitcoin en valor que se almacenan en la cadena de bloques en una dirección de 
Bitcoin específica.

Las entradas especifican qué salidas de transacción gastar, estas entradas hacen referencia a una transacción anterior utilizando el ID de la transacción (txid) y las salidas contienen la cantidad que se enviará así como parte de un programa que contiene un __PKH__, esta parte del programa se denomina __secuencia de comandos pubkey.__ Posteriormente estas salidas se convertirán en una entrada.

Cuando se dice que la billetera de un usuario ha recibido bitcoin, lo que se quiere decir es que la billetera ha detectado una UTXO que se puede gastar con una de 
las claves __(PKH)__ controladas por esa billetera.

Los nodos completos de Bitcoin rastrean todas estás salidas disponibles y gastables y existe una base de datos denominada chainstate que contiene las UTXOs y 
que se utilizará para evitar tener que realizar ciertas búsquedas sobre toda la cadena de bloques.

Así que las __UTXO__ son monedas en Bitcoin que se transfieren de un nodo a otro en toda la red como valor. 

Satoshi Nakamoto en el documento técnico: __Bitcoin: Un Sistema de Efectivo Electrónico Usuario-a-Usuario.__

> *Normalmente habrán o una sola entrada de una transacción previa más grande o múltiples entradas combinando cantidades más pequeñas, y al menos dos salidas: una para el pago, 
> y una para devolver el cambio, si es que hay algún cambio, de vuelta al emisor.*

### ¿Por qué se necesita una tarifa de transacción y cómo se calcula?

Las tarifas de transacción son necesarias para que los mineros procesen las transacciones de los usuarios y que puedan ser incluidas en la cadena de bloques. La tarifa se calcula haciendo una suma de los montos de las entradas, que debe ser mayor o igual que la suma de los montos de las salidas. La diferencia, si la hay, se denomina __tarifa de transacción.__


