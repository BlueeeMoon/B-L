## ¿Qué son las propuestas de mejora de Bitcoin (BIPs) y qué papel juegan en la determinación del protocolo de Bitcoin?

Un BIP (Bitcoin Improvement Proposal) es una propuesta de mejora, un documento de diseño que brinda información para toda la comunidad sobre nuevas funciones, procesos o entorno y existen más de 100.
Estos BIP tienen como objetivo proponer nuevas funciones, documentar decisiones, recopilar información sobre algún problema y existen tres tipos:

- De seguimiento: describe cualquier cambio que afecte a la mayoría de todas las implementaciones.
- Informativo: describe un problema de diseño, sin embargo no propone una nueva característica.
- De proceso: propone un cambio, a menudo requiere el consenso de la comunidad.

Toda esta información está en un BIP, sí, viene en el [__BIP 1__](https://github.com/bitcoin/bips/blob/master/bip-0001.mediawiki),  titulado: __Propósito y lineamientos del BIP__, autor: *Amir Taaki creado en 2011-09-19.*

Por ejemplo el __BIP38__ propone un método para la clave privada protegida con contraseña.

## ¿Por qué se llama a Bitcoin Core la implementación de referencia? ¿Existen otras implementaciones ampliamente utilizadas?

Bitcoin Core es el cliente Bitcoin original y construye la columna vertebral de la red y está principalmente en dos idiomas, `C++` y `Python`, está bajo los términos de la licencia MIT.
Bitcoin Core ha sido la implementación de referencia desde su primera versión. Bitcoin Core incluye un nodo, una interfaz gráfica y una interfaz de línea de comandos.


Bitcoin Core (anteriormente Bitcoin-Qt) es el tercer cliente, desarrollado por Wladimir J. van der Laan basado en el código de referencia original de Satoshi. 
Se incluye con bitcoind desde la versión `0.5.` Bitcoin-Qt ha cambiado de nombre a Bitcoin Core desde la versión `0.9.0.54.`

El cliente Satoshi o el código Satoshi se refiere a `bitcoind`, `bitcoin-client`, `bitcoin-qt` y `Bitcoin Core` . Esto es en honor a Satoshi Nakamoto por crear Bitcoin.
Existen varias implementaciones como:

- [libbitcoin](https://github.com/libbitcoin/libbitcoin-system)
- [bcoin](https://github.com/bcoin-org/bcoin)
- [bitcoinj](https://github.com/bitcoinj/bitcoinj)
- [btcd](https://github.com/btcsuite/btcd)

[Aquí](https://github.com/bitcoinbook/bitcoinbook/blob/develop/ch03.asciidoc#alternative-clients-libraries-and-toolkits) el enlace del libro de __Mastering Bitcoin__ 
dónde puedes ver los clientes, bibliotecas y kits de herramientas alternativos.

## ¿Cuáles son algunas de las razones más comunes por las que usted ejecutaría su propio nodo completo?

#### Es una de las preguntas que mucha gente se hace, considero que aparte de que:

1. Puedes verificar las transacciones.
2. Contribuir a fortalecer la red ayudando a que sea más robusta.
3. Privacidad, seguridad, descentralización. 

Podrás adquirir conocimientos, es decir; una comprensión más profunda sobre él, lo que significa que empezarás a ser un individuo autónomo, libre, responsable, soberano. 

Ejecutar un nodo completo de Bitcoin es la única forma de saber con seguridad que ninguna de las reglas se ha roto. No aceptarías un billete en efectivo o una moneda de oro 
sin verificar que sea genuino, lo mismo se aplica a bitcoin.

## ¿Cuál es la diferencia entre un nodo podado y un nodo completo (también conocido como de archivo)?

#### Un nodo completo:

Un nodo completo de Bitcoin contiene una copia de las salidas de transacciones no gastadas de cada transacción en la cadena de bloques:

- Valida todas las reglas.
- Recibe bloques a medida que se extraen y se propagan.
- Verifica la validez de los bloques.
- Verifica que todas las transacciones en ese bloque sean válidas y estén gastando productos no gastados.
- Hace cumplir las reglas de consenso de la red Bitcoin.

> Un nodo completo tiene dos tipos de datos:
>  - Los bloques tal como fueron serializados, que está almacenando en su disco. 
>  - Un conjunto de salidas de transacciones no gastadas. Lo que necesita para hacer cumplir las reglas de la red es ese conjunto, el conjunto UTXO.
>  
>  El primero son básicamente datos muertos, no lo usa para la validación, y si lo elimina y solo tiene el segundo configurado, aún puede validar todas las reglas.

#### Nodo podado:

Un nodo podado descarga y procesa bloques para construir las bases de datos necesarias para la validación, luego descartan los bloques antiguos para ahorrar 
espacio en disco:

- Es un nodo completo.
- Valida todas las reglas de la red Bitcoin.
- Descarta bloques viejos después de validarlos.
- Ahorra espacio en disco.
- Conserva la historia de dos días.
- Propaga los nuevos bloques. 
- Ve, pero no puede servir viejos bloques a sus compañeros.
















