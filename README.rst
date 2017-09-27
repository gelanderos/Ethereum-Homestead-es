**********************************************************
Guia Homestead de Ethereum
**********************************************************
|Gitter|

.. |Gitter| image:: https://badges.gitter.im/Ethereum-Homestead-es/Ethereum-Homestead-es.svg
   :target: https://gitter.im/Ethereum-Homestead-es?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge

The Ethereum Homestead Guide is the reference documentation accompanying the Homestead release of the Ethereum project.

`Hosted on ReadTheDocs`_

COMO PUEDES AYUDAR?
================================================================================
**INICIATIVA DOCUMENTACION LOCAL DE ETHEREUM**

No importa si eres un principiante o un experto, existen diversas maneras en las que puedes ayudar.

INCLUIR CONTENIDO EN ESTA GUIA
--------------------------------------------------------------------------------
Ayudanos a transferir, traducir y actualizar contenido de la pagina Wiki, de la guia Ethereum Frontier, del Stack Exchange de ethereum o de cualquier otra fuente que pueda proporcionar informacion relevante a esta guia. Alternativamente, puedes escribir tu propio contenido en base a tu propia experiencia.

Asegurate de que la informacion que proporcionas continua siendo exacta y cumple con nuestra guia de contenido ethereum-homestead.readthedocs.org/en/latest/about.html).

REVISA LO QUE YA FUE PUBLICADO
--------------------------------------------------------------------------------
Hecha un vistaso a nuestra guia (https://ethereum-homestead.readthedocs.org/en/latest/) y retroalimentanos visitando nuestra pagina de gitter:(https://gitter.im/ethereum/homestead-guide) o crea un pull request o issue a este repositorio. Facil ¿No?.

¿Y TO QUE GANO?
--------------------------------------------------------------------------------
Tu nombre sera inmortalizado, tanto en nuestros corazones como en nuestra pagina de colaboradores.
Como efecto secundario tambien puede que consigas tener ese sentimiento de satisfaccion que sientes cuando ayudas a la comunidad.

EMPECEMOS
======================

Este proyecto utiliza Sphinx (http://www.sphinx-doc.org/es/stable/index.html) para compilar el codigo html que se publica en Read the Docs. para compilarlo en tu computadora, deberas hacer lo siguiente:

PREREQUISITOS
--------------------------------------------------------------------------------
* Python 2.6 o mayor
* git

Instalar Sphinx, etc
--------------------------------------------------------------------------------
Para usuarios de OSX/Linux (Basandonos en las instrucciones aqui descritas: https://read-the-docs.readthedocs.org/en/latest/getting_started.html). la version de Sphinx 1.4.0 ya no instala de manera automatica `sphinx_rtd_theme`, por esto añadimos las instrucciones para instalarlo de manera adicional.

* Desde la linea de comandos: ``sudo pip install sphinx sphinx_rtd_theme``

Para usuarios de Windows:

* http://www.sphinx-doc.org/en/stable/install.html#windows-install-python-and-sphinx

Obtener el Codigo Fuente
--------------------------------------------------------------------------------
* git clone: https://github.com/ethereum/homestead-guide.git

Compilar y ver el html
--------------------------------------------------------------------------------
* En una ventana de la terminal, ingresa al directorio en donde clonaste el repositorio Guia de Documentacion Local de Ethereum y digita los siguientes comandos:.
* ``make html``
* ``cd build/html``
* ``open index.html`` (abrir en el explorador)
* Pista: cada vez que corras el comando ``make html``, solo actualiza tu ventana del explorador para ver los cambios.


Recursos
================================================================================

**Documentacion**

* Homestead Guide online: https://ethereum-homestead.readthedocs.org/en/latest/index.html
* Github: https://github.com/ethereum/homestead-guide
* Gitter: https://gitter.im/ethereum/homestead-guide
* Google doc: https://docs.google.com/document/d/1rVjrNgaDRAQdPp4rGqWrEk5fPgiHff0xsYGCyf06oM8/edit

**Documentacion Original**

* Wiki de Ethereum: https://github.com/ethereum/wiki/wiki
* Guia Frontier: https://ethereum.gitbooks.io/frontier-guide/content/ (see below for converted files)
* Enorme lista de recursos de Souptacular: https://souptacular.gitbooks.io/ethereum-tutorials-and-tips-by-hudson/content/giant_ethereum_resource_list.html

**Read the Docs y Sphinx**

- Read the Docs: https://read-the-docs.readthedocs.org/en/latest/getting_started.html
- Sphinx docs: http://www.sphinx-doc.org/es/stable/contents.html
- reStructuredText Primer: http://www.sphinx-doc.org/es/stable/rest.html
- RST cheat sheet: https://github.com/ralsina/rst-cheatsheet/blob/master/rst-cheatsheet.rst

Estructura del directorio
=========================

.. code-block::

    homestead-guide
      build    - Directorio de trabajo, no esta presente en el repo
      source   - contenido web en formato rst
        conf.py - archivo de configuracion de sphinx
      old-docs-for-reference (documentacion de la "frontier era")
        wiki    - wiki de the legacy
        gitbook - recursos del gitbook de the legacy (convertidos a rst)
      make.bat - Script de windows para compilar los documentos.
      Makefile - archivo de make para compilar los documentos


Acerca de este repositorio
================================================================================

Este repositorio es unicamente una traduccion del original que se puede encontrar en la siguiente pagina:

.. _Hosted on ReadTheDocs: http://ethereum-homestead-es.readthedocs.io/en/latest/
