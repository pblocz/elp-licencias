---
layout: default
---
# Licenciar tu código

Una de las cosas más importantes a la hora de lanzar un proyecto de
programación es decidir bajo que licencia se abre, fundamental para
garantizar que el dueño del proyecto puede mantenerlo.

Para ello, es recomendable usar una licencia aprobada por la *Open
Source Initiative*. ¿Por qué es esto? Porque son las más extendidas y
es más probable que los potenciales usuarios y contribuyentes a
nuestro proyectos las entiendan. Usar otro tipo de licencias o crear
tú una te quita estas ventajas.


## ¿Cómo elegir la licencia?

Hay varias licencias, y la que elijas dependerá de los intereses que
tengas para el proyecto. Hay algunas páginas que te ayudan a elegir,
por ejemplo [What Kind Of Licence Should I Choose?][whatlicence]

Las licencias libres más comunes y que cubren un gran espectro de casos de uso son:

- **MIT**: Licencia muy corta, simple y permisiva. Sería un
  equivalente a *CC BY* en términos de permisividad y sin garantías de
  uso.

- **Modified BSD**: Equivalente a la licencia **MIT**, pero haciendo
  explícito que no se puede usar el nombre, marca o logo de los
  contribuidores o del programa.

- **Mozilla Public License**: Termino medio entre la licencia **BSD
  Modificada** y la **GPL**. A lo que especifica la licencia **BSB**
  se añade que si se distribuye el software, el código fuente también
  hay que distribuirlo.

- **GPL**: La licencia libre por excelencia que obliga a liberar el
  código al igual que la MPL, informar de cambios en el código e
  impide crear licencias que sean más privativas que la **GPL**.

## Poner licencia al código

Es importante seguir correctamente los pasos y referenciar de manera
clara y sin ambigüedad la licencia, para prevenir futuros problemas
legales. Cada licencia tiene su proceso concreto, pero en rasgos
generales bastaría con lo que explicamos a continuación.

### Propiedad del código

Una vez que hemos decidido la licencia más apropiada, tenemos que
asegurarnos de que podemos probar legalmente lo que exige la
licencia. En concreto, debemos poder asegurar legalmente que:

- El código es exclusivamente de nuestra propiedad intelectual.
- Tenemos todos los derechos necesarios para licenciarlo como
  deseamos.
- Supervisar (auditing) el proyecto de manera continuada para
  asegurarse que se mantiene la licencia y autoría del código.

En proyectos pequeños, es más fácil asegurar que el código es exclusivamente propiedad intelectual del dueño. Proyectos más grandes pueden haber recibido contribuciones de personas externas al proyecto, como un contratista o alguien que ha donado código, y no tener los derechos sobre ese trabajo explícitamente.


Es importante definir un proceso de auditoría continuada de la
propiedad intelectual. Es aconsejable definir un mecanismo y
herramientas que permitan saber en cada momento quién ha hecho qué,
para llevar un control del desarrollo y evitar problemas como disputas
o litigios sobre la propiedad del código.

### Pasos a seguir

Debemos aplicar la licencia de manera que la gente pueda verla. No es
suficiente con afirmar que tu código está disponible bajo una licencia
determinada, sino también que es visible en todas las localizaciones
apropiadas. Han de llevarse a cabo las siguientes acciones, como
mínimo requerido:

- **Especificar la licencia** seleccionada en tu página web
  (preferiblemente en la página principal como en la de descargas)
- Proveer el **texto íntegro de la licencia** en la página web y en el
  directorio raíz del código fuente de tu proyecto (Usualmente llamado
  LICENSE.TXT)
- Proveer un **texto modelo en el encabezado de cada archivo del
  código** del proyecto. Este texto modelo varía de licencia a
  licencia.
- Proveer el texto completo de la licencia en el directorio raíz de
  todo aquello que no sea código.

Por supuesto, hay que poner a disposición de la gente formas de
descarga y/o contribución al proyecto, por ejemplo, o desde puntos de
distribución como Github , Google Code o SourceForge, además de
incluir información de contacto, por ejemplo en el archivo README.


### Aviso de copyright

Es importante añadir correctamente el aviso al encabezado de cada
archivo, para hacerlo, hay que seguir unos pasos que depende cada una
de las licencias, aunque al añadirla hay que tener en cuenta 2 cosas:
el aviso de copyright y la declaración de los permisos de copyright,
indicando bajo qué licencia está distribuido el programa.

El aviso de copyright debería incluir el año (o rango de años) en que
se terminó de preparar el lanzamiento. Si varias personas ayudaron a
escribir el código, hay que usar todos sus nombres.

Un ejemplo extraído de la [licencia MPL](https://www.mozilla.org/MPL/boilerplate-1.1/):

	/* ***** BEGIN LICENSE BLOCK *****
	* Version: MPL 1.1
	*
	* The contents of this file are subject to the Mozilla Public License Version
	* 1.1 (the "License"); you may not use this file except in compliance with
	* the License. You may obtain a copy of the License at
	* http://www.mozilla.org/MPL/
	*
	* Software distributed under the License is distributed on an "AS IS" basis,
	* WITHOUT WARRANTY OF ANY KIND, either express or implied. See the License
	* for the specific language governing rights and limitations under the
	* License.
	*
	* The Original Code is __________________________________________.
	*
	* The Initial Developer of the Original Code is
	* ____________________________________________.
	* Portions created by the Initial Developer are Copyright (C) 2___
	* the Initial Developer. All Rights Reserved.
	*
	* Contributor(s):
	*
	* ***** END LICENSE BLOCK ***** */


Un ejemplo más sencillo que se podría usar en caso de que la licencia lo permita y los que han contribuido al código ya estén reflejados en otro lugar, por ejemplo en un control de versiones como git:

	/*! Nombre_del_proyecto vX.Y
	Copyright (c) 2010-2014 nombre_de_los_dueños_originales

	This Source Code Form is subject to the terms of the
	Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
	with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
	*/


Si se ha copiado código de otras personas bajo la misma licencia,
deben copiarse sus avisos de copyright también. Así, se pondrán todos los
avisos juntos al principio de cada archivo, o en un archivo auxiliar al que se haga referencia desde el aviso de copyright.


<!--
### Las licencias GPL

Al añadir una licencia hay que tener en cuenta 2 cosas: el aviso de
copyright y la declaración de los permisos de copyright, indicando
bajo qué licencia está distribuido el programa.

El aviso de copyright debería incluir el año (o rango de años) en que
se terminó de preparar el lanzamiento. Si varias personas ayudaron a
escribir el código, hay que usar todos sus nombres.

Tanto si el programa se libera bajo una licencia GPL o LGPL, se debe
incluir una versión de texto de la licencia. En los programas GNU la
licencia GPL se encuentra normalmente en un archivo llamado
COPYING. En el caso de LGPL, el archivo se llamará COPYING.LESSER.

Si se ha copiado código de otras personas bajo la misma licencia,
deben copiarse sus avisos de copyright. Así, se pondrán todos los
avisos juntos al principio de cada archivo.


Además es importante incluir información de contacto, por ejemplo en
el archivo README.


La declaración de los permisos de copyright debería incluirse justo
después de los avisos de copyright. Un ejemplo de GPL sería el
siguiente:

>This program is free software: you can redistribute it and/or modify
>it under the terms of the GNU General Public License as published by
>the Free Software Foundation, either version 3 of the License, or
>at your option) any later version.
>
>This program is distributed in the hope that it will be useful,
>but WITHOUT ANY WARRANTY; without even the implied warranty of
>MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
>GNU General Public License for more details.
>
>You should have received a copy of the GNU General Public License
>along with this program.  If not, see <http://www.gnu.org/licenses/>.


Para programas interactivos se recomienda mostrar por pantalla
brevemente un aviso sobre el copyright y los permisos de copia al
iniciarse el programa.

-->

## Licenciar el contenido

No obstante, no solo hay que tener en cuenta la licencia del código
(las licencias libres u open source son para software), también las
licencias de las imágenes, sonidos y documentos que contenga el
proyecto. Se recomienda *Creative Commons*.  De igual forma, también
se necesita tener una licencia para las bases de datos.


## Incluir código libre en tu proyecto

Si tu código incluye librerías de otros proyectos es importante que tu
licencia se adecúe a las de estos. Por lo tanto, hay que considerar si
las licencias de cada una de las librerías son compatibles con la
nuestra.

Diferentes licencias requieren diferentes atribuciones, por lo que la
decisión más sencilla es tratarlas a todas igual, ya que dar más
atribuciones de las necesarias no suele ser un problema. Es común
incluir un texto NOTICE.txt en la raíz del directorio indicando la
información importante sobre las licencias de las librerías que usas.

Es importante puntualizar que hay una licencia con requisitos particulares: Common Public Attribution License

Además de incluir las licencias de las librerías se deberá incluir la
licencia de cada componente de código usada en el proyecto. Se suele
incluir el texto completo de la licencia de cada componente en el
directorio donde se encuentra. También es importante mantener las
cabeceras de licencia de los archivos, aunque esto puede ser obligatorio o no dependiendo de la licencia usada.

## Formas de negocio

Una alternativa bastante usual, pensando en sacarle provecho económico al proyecto,  es liberar tu código usando una doble licencia.

Es decir, el software se lanza bajo una licencia copyleft fuerte y lanzar otra versión alternativa, que no contenga copyleft, para aquellos usuarios con los que se quiera llegar a un acuerdo, que estén interesados en desarrollar proyectos basados en el código pero no quieran estar limitados para una licencia copyleft.

Para hacer esto, hay que tener en cuenta que o tienes el copyright de todos los componentes del software o bien los distintos desarrolladores están de acuerdo en liberarlo bajo esa licencia.

## Enlaces de interés

- Explica la importancia de mantener una lista de contribuyentes a un
  proyecto [[https://www.softwarefreedom.org/resources/2012/...][softwareblame]]

- Open Source Initiative [[http://www.opensource.org/](http://www.opensource.org/)]
- Free Software Foundation [[http://www.fsf.org/](http://www.fsf.org/)]
- Manteniendo Archivos de Licencia Permisivos en un proyecto GPL: Guía para Desarrolladores.[[http://www.softwarefreedom.org/resources/2007/gpl-non-gpl-collaboration.html][srfm]]
- Creative Commons [[http://creativecommons.org/](http://creativecommons.org/)]
- Licencias Open database  [[http://opendatacommons.org/licenses/](http://opendatacommons.org/licenses/)]
- Cómo aplicar la licencia GPL [[http://www.gnu.org/licenses/gpl-howto.html][gplhowto]]
- Introducción al desarrollo de código libre [[http://oss-watch.ac.uk/resources/iprguide][licenseintro]]

[srfm]: <http://www.softwarefreedom.org/resources/2007/gpl-non-gpl-collaboration.html>
[openyourcode]: <http://oss-watch.ac.uk/resources/opensourceyourcode>
[licenseintro]: <http://oss-watch.ac.uk/resources/iprguide>
[whatlicence]: <http://oss-watch.ac.uk/resources/licdiff>


[chooselicense]: <http://choosealicense.com/licenses/>
[gplhowto]: <http://www.gnu.org/licenses/gpl-howto.html>
[softwareblame]: <https://www.softwarefreedom.org/resources/2012/ManagingCopyrightInformation.html>
