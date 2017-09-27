.. _what-is-ethereum:

################################################################################
¿Que es Ethereum?
################################################################################

Ethereum es una plataforma de blockchain de codigo abierto que permite a cualquier persona construir y utilizar aplicaciones descentralizadas que son ejecutadas mediante la tecnologia de la misma blockchain. Al igual que con el Bitcoin, nadie puede controlar controls o ser dueño de la red Ethereum –  es un proyecto de codigo abierto construido por una gran cantidad de personas alrededor del planeta. Pero al contrario del protocolo del Bitcoin, Ethereum se diseño para ser adaptable y flexible.  Entre sus muchas virtudes esta el hecho de que se pueden crear facilmente nuevas aplicaciones en la plataforma de Ethereum, y con la actualizacion "Homestead", es seguro para cualquier persona utilizar dichas aplicaciones.

================================================================================
Una red blockchain de siguiente Generacion
================================================================================

La tecnologia Blockchain es la base tecnologica del bitcoin, mencionada por primera vez por su misterioso autor "Satoshi Nakamoto" (cuya real identidad es desconocida) en su documento tecnico llamado"Bitcoin: A Peer-to-Peer Electronic Cash System"(Bitcoin: un sistema de dinero electronico de Igual a Igual o P2P), publicado en 2008. Mientras la implementacion de las blockchain para usos mas generales se discutia en el documento original, no fue hasta algunos años despues que las blockchains  emergieron como un termino generico. Una blockchain es una arquitectura computacional distribuida donde todos los nodos de la red ejecutan y almacenan las mismas transacciones, las cuales estan agrupadas en blockes. Solo un bloque puede ser añadido cada determinado tiempo, y cada bloque contiene una prueba matematica que verifica que este continua con la secuencia del bloque anterior. De esta manera, la "Base de datos distribuida" de la blockchain se mantiene en concenso a lo largo de toda la red. Las transacciones de los usuarios en lo individual con los libros de la plataforma son aseguradas mediante fuertes algoritmos criptograficos. Los nodos que mantienen y verifican la red son incentivados con incentivos economicos matematicamente blindados codificados en el protocolo.

En el caso del Bitcoin, la base de datos esta concebida como una tabla de cuentas y balances denominado "ledger" o libro contable, y las transferencias son transacciones de bitcoin realizada dentro del mismo libro para asegurar finanzas libres de la necesidad de confiar en terceros. Pero ya que el caso del Bitcoin comenzo a atraer una mayor atencion de parte de los desarrolladores y tecnologos, proyectos importantes comenzaron a hacer uso de la red de este para propositos diferente a las transferencias de monedas valuables. Muchos de estos tomaron la forma de "alt coins" o monedas alternas - blockchains con monedas criptograficas o electronicas propias, las cuales mejoraron el protocolo original añadiendo nuevas funciones o capacidades. En los ultimos meses del 2013, El inventor de Ethereum inventor Vitalik Buterin propuso que una unica blockchain con la capacidad de ser reprogramada para realizar cialquier especie de calculo complejo, esta podria englobar todos esos otros proyectos.

En 2014 los fundadores de Ethereum, Vitalik Buterin, Gavin Wood and Jeffrey Wilcke comenzaron a trabajar en la blockchain de proxima generacion que tenia la ambicion de implementar una plataforma para contratos inteligentes general y libre de necesidad de confianza.

================================================================================
La Maquina Virtual de Ethereum o "EVM"
================================================================================

Ethereum es una blockchain programable. La cual en lugar de ofrecer a los usuarios un ciertas operaciones pre definidas (Por ejemplo las transacciones de bitcoin) Ethereum permite a los usuarios crear operaciones de cualquier complejidad que ellos deseen. De esta manera, esta funciona como una plataforma para varios diferentes tipos de aplicaciones descentralizadas basadas en la blockchain, incluyendo pero no limitado a criptomonedas.

Ethereum en su mas estricto sentido se refiere a una suite de protocolos que definen una plataforma ideal para aplicaciones descentralizadas. En el corazon de esta se encuentra la Maquina Virtual de Ethereum o mejor conocida como :ref:`Ethereum Virtual Machine ("EVM") <the-EVM>`, la cual puede ejecutar codigo de complejidad algorithmica de manera arbitraria. En terminos de ciencias de la computacion, Ethereum es "Turing complete" o Touring completo, lo que significa que teoricamente podria resolver cualquier problema computacional razonable. Los desarrolladores pueden crear aplicaciones que se ejecutan en la Maquina Virtual de Ethereum usando lenguajes de programacion amigables modelados en lenguajes existentes como JavaScript y Python.

Como cualquier otra blockchain, Ethereum  tambien incluye un protocolo de red P2P o de Igual a Igual. La base de datos de la blochain de Ethereum es mantenida y actualizada por una gran cantidad de nodos conectados a la red. todos y cada uno de los nodos en la red de ethereum ejecutan la Maquina Virtual de Ethereum y ejecutan las mismas instrucciones. Por esta razon, algunas veces Ethereum es llamada la Computadora mundial o en ingles "World computer".

Esta paralelizacion masiva de poder computacional a lo largo de toda la red de Ethereum no se realiza para volver la computacion mas eficiente. De hecho, este proceso hace la computacion en Ethereum mucho mas lenta y costosa que en una "computadora" tradicional. En lugar de esto, cada nodo de Ethereum ejecuta la Maquina Virtual de Ethereum para mantener un consenso a traves de toda la blockchain. El consenso descentralizado otorga a Ethereum muy altos niveles de tolerancia ante errores, asegura que la red nunca se encuentre inactiva y vuelve la informacion almacenada en la blockchain imposible de modificar y resistente a la censura.

La plataforma de Ethereum por si sola no cuenta con ningnuna adicional ni ningun valor. Sin embargo, de manera similar a un lenguaje de programacion, esta en manos de los desarrolladores y emprendedores decidir para que debe ser usada. Sin embargo, esta claro que algunos tipos de aplicaciones se benefician mas de la plataforma Ethereum que otros. Especificamente, ethereum esta hecha para  **aplicaciones que automatizan interacciones directas entre iguales o facilitan la organizacion de grupos dentro de una red**. por ejemplo, aplicaciones para coordinar tiendas donde se venden productos entre iguales, o la automatizacion de contratos financieros complejos. el Bitcoin permite a individuos realizar transacciones economicas sin la necesidad de intermediarios como son las instituciones financieras, bancos o los gobiernos. mas el impacto de Ethereum puede tener un mayor alcance. En teoria, las interacciones financieras o los cambios de cualquier nivel de complejidad podrian ser llevados acabo de manera automatica y confiable usando codigo que se ejecuta en Ethereum. Ademas de las aplicaciones financieras, cualquier situacione en la que la confianza, seguridad y permanencia son importantes – por ejemplo, registros de activos, votaciones, gobierno, y el internet de las cosas "IoT" – podrian ser impactados de manera positiva por la plataforma de Ethereum.

================================================================================
¿Como funciona Ethereum?
================================================================================

Ethereum incorpora una gran cantidad de funciones y tecnologias que le resultaran familiares a los usuarios de Bitcoin, mientras que tambien se añaden muchas modificaciones e innovaciones propias.

Al tiempo que la blockchain de Bitcoin era unicamente una lista de transacciones, :ref:`la unidad basica de Ethereum es la cuenta o "Account" <Accounts>`. la blockchain de Ethereum rastrea el estado de todas las cuentas, y todas las transiciones de estado en la blockchain son transferencias de valores e informacion entre las cuentas. Actualmente existen dos tipos de cuentas:

- Cuentas propiedad de externos o (EOAs) Externally Owned Accounts, las cuales son administradas con claves privadas.
- Cuentas basadas en Contratos, las cuales son controladas y administradas por el codigo de sus contratos y unicamente pueden ser activadas por una cuenta propiedad de externos o ("EOAs")

Para la mayoria de los usuarios, la diferencia entre estas es que los humanos manejan las EOAs porque pueden controlar las claves privadas lo cual otorga control sobre las mismas. Las cuentras contrato, en la otra mano, son gobernadas por su codigo interno. Si son controladas por un usuario humano, es porque estan programadas para ser controladas por un EOA con una cierta direccion preestablecida, la cual es controlada por quien sea que tenga la llave privada que controla esa multicitada EOA. El termino popular "Contratos Inteligentes" o "smart contracts" hace referencia a un codigo en la cuenta contrato – programas que se ejecutan cuando una transaccion es enviada a esa cuenta. Los usuarios pueden crear contratos nuevos desplegando codigo hacia la blockchain.

Al igual que con el Bitcoin, los usuarios deben pagar pequeñas comisiones por transaccion a la red. esto proteje la red de ethereum de tareas computacionales maliciosas como son los Ataques de Denegacion de Servicios o "DDoS" y los bucles infinitos. El remitente de una transaccion debe pagar por cada paso del programa que activaron incluyendo el poder computacional y memoria de almacenamiento.  Estas comisiones son pagaderas en la moneda Moneda de Valor nativa de Ethereum denominada, ether.

Estas transacciones son recolectadas por los nodos que validan las transacciones. Estos "mineros" son nodos en la red de ethereum que reciben, propagan, verifican y ejecutan transacciones. Los mineros agrupan las transaciones, las cuales incluyen actualizaciones a el estado de las cuentas dentro de la blockchain de ethereum – lo que se llama "bloques", y los mineros compiten entre unos y otros para que su bloque sea el siguiente en ser añadido a la cadena. Los mineros son recompensados con ether por cada bloque efectivamente minado. Esto provee un incentivo economico para la gente que dedica hardware y energia electrica a la red de ethereum.

Tal como en la red de bitcoin Bitcoin, los mineros tienen la tarea de resolver problemas matemaricos complejos para poder minar un bloque satisfactoriamente. Esto es conocido como Prueba de Trabajo o "Proof of Work". Cualquier problema computacional que requiere mas recursos en ordenes de magnitud mayores para resolver algoritmos que los requeridos para verificar es un buen candidato para prueba de trabajo. Para desalentar la centralisation debido al uso de hardware especializado por ejemplo ASICs, como ocurrio en la red de Bitcoin, Ethereum eligio un problema computacional  dificil de memoria. Si el problema requiere una gran cantidad de memoria ademas de cpu, el hardware ideal es, de hecho, cualquier computadora ordinaria. Esto vuelve al algoritmo de prueba de trabajo de ethereum resistente a ASICs, permitiendo una distribucion mas descentralizada de seguridad que la de las blockchains en las cuales la mineria esta dominada por hardware especializado como el Bitcoin.


Aprende acerca de Ethereum (Recursos en ingles)
==============================

[to be extended]

Videos de PR con algunos pathos:
---------------------------------

* `Ethereum: the World Computer <https://www.youtube.com/watch?v=j23HnORQXvs>`_
* `Ethereum -- your turn <https://vimeo.com/88959651>`_


Blockchain y Ethereum 101
----------------------------------

* `Explain bitcoin like I'm five <https://medium.com/@nik5ter/explain-bitcoin-like-im-five-73b4257ac833>`_ - an excellent introduction to blockchain technology and bitcoin to the mildly techsavvy layperson.
* https://medium.com/@creole/7-a-simple-view-of-ethereum-e276f76c980b
* https://blog.chain.com/explaining-ethereum-fd043c7d602e

* `Explain Ethereum to non-technical people Q&A on stackexchange <http://ethereum.stackexchange.com/questions/45/how-would-i-explain-ethereum-to-a-non-technical-friend>`_
* Reddit threads on ELI5-ing Ethereum:

`[1] <https://www.reddit.com/r/ethereum/comments/43brik/explaining_ethereum_to_friends/>`_
`[2] <https://www.reddit.com/r/ethereum/comments/3c132d/eli5_what_you_guys_do_here/>`_
`[3] <https://www.reddit.com/r/ethereum/comments/1vvz13/eli5_ethereum/>`_
`[4] <https://www.reddit.com/r/ethereum/comments/1vb1gc/is_ethereum_an_alt_coin_can_anyone_eli5/>`_
`[5] <https://www.reddit.com/r/ethereum/comments/4279dh/eli5_what_exactly_is_ethereum/>`_
`[6] <https://www.reddit.com/r/ethereum/comments/2hl10p/eli5_ethereum/>`_
`[7] <https://www.reddit.com/r/ethereum/comments/41y8by/the_best_way_i_can_eli5_ethereum_to_someone/>`_
`[8] <https://www.reddit.com/r/ethereum/comments/44b69e/i_dont_understand_the_technology/>`_
`[9] <https://medium.com/@nik5ter/explain-bitcoin-like-im-five-73b4257ac833>`_
`[10] <https://www.reddit.com/r/ethereum/comments/1vb1gc/is_ethereum_an_alt_coin_can_anyone_eli5/>`_
`[11] <https://www.reddit.com/r/ethereum/comments/2dpgwy/eli5_ethereum/>`_
`[12] <https://www.reddit.com/r/ethereum/comments/47u5y9/explain_what_ethereum_is_to_a_bitcoin_trader/>`_
`[13] <https://www.reddit.com/r/ethereum/comments/27wsgq/eli5_ethereum_its_uses_its_features_its_future/>`_
`[14] <https://www.reddit.com/r/ethereum/comments/4936d3/are_you_new_to_ethereum_here_are_many/>`_
`[15] <https://www.reddit.com/r/ethereum/comments/4279dh/eli5_what_exactly_is_ethereum/>`_
`[16] <https://www.reddit.com/r/ethereum/comments/3n37dp/explaining_ethereum_ecosystem_for_normal/>`_
`[17] <https://www.reddit.com/r/ethereum/comments/271qdz/can_someone_explain_the_concept_of_gas_in_ethereum/>`_
`[18] <https://www.reddit.com/r/ethereum/comments/3hg7id/why_should_the_average_person_care_about_ethereum/>`_
`[19] <https://www.reddit.com/r/ethereum/comments/43exre/what_are_the_advantages_of_ethereum_over_other/>`_


Videos
----------------------

* http://change.is/video/ethereum-the-world-computer-featuring-dr-gavin-wood

Infografias
--------------------------------

* `Ethereum explained...[to your mother] <https://blog.ethereum.org/wp-content/uploads/2015/06/Ethereum-image-infographic-beginners-guide.png>`_
* http://decentral.ca/wp-content/uploads/2016/03/infographic.jpg
* https://medium.com/@angelomilan/ethereum-explained-to-my-mom-infographic-673e32054c1c#.n9kzhme6v


Comparacion con las alternativas
---------------------------------

* `NXT <https://www.reddit.com/r/ethereum/comments/23aejv/eli5_what_is_the_qnce_between_ethereum_and/>`_
* `MaidSafe <https://www.reddit.com/r/ethereum/comments/22r49u/how_is_maidsafe_different_then_etherium/>`_
