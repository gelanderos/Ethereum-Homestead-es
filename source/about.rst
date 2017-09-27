***************************************
Guia Homestead de Ethereum
***************************************
|Gitter|

.. |Gitter| image:: https://gitter.im/Ethereum-Homestead-es/Lobby.svg
   :target: https://gitter.im/Ethereum-Homestead-es/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
===============================================================================
Este proyecto es derivado del proyecto "Ethereum Homestead Documentation" que consiste por una parte en la traduccion de los documentos incluidos en dicho repositorio, sin embargo por otro lado se pretende la alimentacion de este nuevo repositorio con informacion totalmente nueva y en español.
***************************************
Introduccion
***************************************

Proposito y Audiencia
===============================================================================

Esta guia tiene la finalidad de inicializar a los usuarios y desarrolladores interesados en el mundo de Ethereum.
La meta es crear documentacion con informacion, pequeños tutoriales y ejemplos que cubran todas las funcionalidades basicas e intermedias de Ethereum para interactuar con, o desarrollar "DAPPS".

Cualquier informacion que es demaciado especifica, tecnica o no necesaria para cumplir con el objetico de la documentacion permanecera en la pagina Wiki de nuestro Github el cual podra ser referenciado en esta guia si se considera necesario.

En los apartados de la izquierda en esta guia podras tambien encontrar informacion acerca de la actualizacion "Frontier" de ethereum, pedimos a quienes redacten alguno de los documentos aqui publicados que hagan su mayor esfuerzo para asegurarse de que la informacion importada continúe siendo precisa.
Esta guia no esta enfocada a ningun cliente y/o sistema operativo en especifico, por lo que los ejemplos y tutoriales pueden estar basados en cualquier cliente de Ethereum que el autor decida utilizar, esto siempre y cuando el autor haga la distincion de cual cliente esta siendo utilizado en el ejemplo o tutorial.

A pesar de que en las primeras versiones de esta guia no se incluira informacion demasiado tecnica y/o especifica, el uso y popularidad de esta guia entre la comunidad marcara la pauta a futuras deciciones, entre las cuales puede encontrarse mover la informacion de la pagina de wiki de nuestro github repo a este formato.

Ejemplos de informacion demasiado tecnica y/o especifica incluyen pero no estan limitados a:

* ETHash, CASPER, ABI, RLP, y otras especificaciones tecnicas.
* Especificaciones completas de APIs para protocolos. Advertencia: en los ejemplos, si la informacion o tutoriales necesitan hacer referencia a alguna llamada a una API para un cliente o una interface para poder concluir su ejemplo sera aceptable referenciar la llamada especifica requerida. Asegurate de  realizar una llamada de la que el usuario aun pueda encontrar informacion especifia sobre su uso en el Wiki de nuestro github.

Recursos para documentacion ejemplar
===============================================================================

Estos son algunos de los ejemplos de documentacion anterior de Ethereum asi como ejemplos de documentacion ejemplar, estos se encuentran redactados en ingles, sin embargo se puede detectar facilmente la estructura e informacion que en ellos se detalla.

* Solidity Docs - https://ethereum.github.io/solidity/docs/home/
* Frontier Guide - https://ethereum.gitbooks.io/frontier-guide/content/
* Gav’s TurboEthereum Guide - https://gavofyork.gitbooks.io/turboethereum/content/
* Ancient EthereumBuilder’s Guide - https://ethereumbuilders.gitbooks.io/guide/content/en/index.html
* Other Ethereum Links: https://souptacular.gitbooks.io/ethereum-tutorials-and-tips-by-hudson/content/giant_ethereum_resource_list.html
* Django Docs - https://docs.djangoproject.com/en/1.9/

Restructured Text Markup, Sphinx
=======================================

* Best Cheat Sheet - https://github.com/ralsina/rst-cheatsheet/blob/master/rst-cheatsheet.rst
* Quick Reference - http://docutils.sourceforge.net/docs/user/rst/quickref.html
* Official Cheat Sheet - http://docutils.sourceforge.net/docs/user/rst/cheatsheet.txt -> http://docutils.sourceforge.net/docs/user/rst/cheatsheet.html
* RST Primer http://sphinx-doc.org/rest.html
* http://sphinx-doc.org/markup/inline.html

Compilacion y Despliegue
===============================================================================

Nosotros utilizamos `make` con el `Makefile` generado por read-the-docs para construir el documento.

.. code-block:: bash

    git clone https://github.com/ethereum/homestead-guide
    cd homestead-guide
    make html

Tips para el procesamiento
===============================================================================

Fija las lineas delimitadoras de secciones, (procura utilizar siempre lineas de 80 caracteres de longitud para tener la longitud correcta, esto, a menos que cuentes con titulos aun mas largos)

.. code-block:: bash

    for f in `ls source/*/*.rst`; do cat $f|perl -pe 's/\=+$/================================================================================/' > $f.o; mv $f.o $f; done; done
    for f in `ls source/*/*.rst`; do cat $f|perl -pe 's/\*+$/********************************************************************************/' > $f.o; mv $f.o $f; done
    for f in `ls source/*/*.rst`; do cat $f|perl -pe 's/\-+$/--------------------------------------------------------------------------------/' > $f.o; mv $f.o $f; done
    for f in `ls source/*/*.rst`; do cat $f|perl -pe 's/\++$/++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++/' > $f.o; mv $f.o $f; done
    for f in `ls source/*/*.rst`; do cat $f|perl -pe 's/\#+$/################################################################################/' > $f.o; mv $f.o $f; done

Referenciando documentacion antigua
===============================================================================

La carpeta "old-docs-for-reference" tiene todos los documentos de  la actualizacion frontier incluyendo el "Gitbook" y el wiki de Ethereum. Sientete libre de copiar y pegar informacion que aun se considera relevante de dichos archivos.

Migrar y convertir contenido de el wiki antiguo utilizando Pandoc
===============================================================================

Si aun quieres clonar las ultimas versiones del wiki de ethereum y la guia de la actualizacion frontier originales mismas que se encuentran redactadas en ingles, puedes utilizar los siguientes comandos:

.. code-block:: bash

    git clone git@github.com:ethereum/go-ethereum.wiki.git
    git clone git@github.com:ethereum/wiki.wiki.git

    mkdir main-wiki.rst
    mkdir go-ethereum-wiki.rst

    for f in `ls wiki.wiki/*.md`; do pandoc $f -o main-wiki.rst/`basename $f .md`.rst; done
    for f in `ls go-ethereum.wiki/*.md`; do pandoc $f -o go-ethereum-wiki.rst/`basename $f .md`.rst; done
