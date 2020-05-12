# TicketAI

- [Generalidades](#Generalidades)
- [Cargar_Archivos](#Cargar_Archivos)
- [Buscar](#Buscar)
- [Documentos](#Documentos)
- [Detalles_Documento](#Detalles_Documento)

# Generalidades

TicketAI es una herramienta diseñada con un complejo algoritmo de “Machine Learning” que permite la lectura inteligente de tickets. 

Las capacidades de lectura son la base, de un sistema de manejo de información enfocado en obtener bases de datos solidas que permitan explotar la información recopilada en los tickets. 

## Funcionalidades

TicketAI cuenta con las siguientes funcionalidades: 

* Documentos; 
* Cargar Archivos; y 
* Buscar

Para explicar	a detalle las funcionalidades, se tienen secciones dedicadas a cada una de ellas. 

## ¿Seguridad? 

## Últimas Mejoras

# Cargar_Archivos

A nivel de procedimiento, esté sería el primer paso por seguir, es la carga de archivos.

TicketAI, tiene diferentes bondades al momento de cargar archivos, en los siguientes puntos se describirán con detenimiento.

## Tipos de Archivos Permitidos

TicketAI permite cargar los siguientes archivos en su sistema:

- Archivos .jpg
- Archivos .png


Bajo la idea de que un ticket escaneado sea equivalente a un archivo, este proceso puede tomar mucho tiempo en concretarse, por lo tanto, para facilitar esta carga de archivos, TicketAI permite:

- Archivos .zip
- Archivos .tar

## Flujo de Trabajo

A continuación, se muestra el flujo de trabajo para realizar la carga de archivos en TicketAI:

![Cargar Documentos](https://user-images.githubusercontent.com/63880141/80722746-56f04a00-8ac5-11ea-8201-4af6a0afacd4.png)

### Precisiones Referentes al Flujo de Trabajo

Login: Acceso a la Plataforma

1.	Menú: El menú es el botón de la esquina superior izquierda.

2.	Cargar Archivo: Es una funcionalidad que se despliega al dar clic en el botón Menú.

3.	¿Se cargaron los archivos?: La Pantalla muestra un cuadro con la leyenda: "Arrastre los Archivos aquí", al arrastrar los archivos se muestra una imagen del archivo cargado.

3.1	 Si los archivos no se cargan correctamente aparece un icono rojo de rechazo.

3.2	 Si los archivos se cargan correctamente aparece un icono verde de confirmación.

4.	Eliminar Archivo: Una de las bondades que tiene TicketAI es permitirnos remover algún archivo que erróneamente hubiera sido cargado.

4.1	Si no desea remover ningún archivo, aquí termina el proceso.

4.2	Si desea eliminar algún archivo, se debe colocar el puntero del mouse sobre el archivo cargado que desee eliminar y dar clic en la opción “Eliminar Archivo”

## Recomendaciones Adicionales

1. Si un ticket está muy maltratado, roto o con varios sellos o firmas encima podría no ser interpretado correctamente por el sistema.

2. La calidad mínima de un ticket escaneado es: 600 dpi.

## Los Archivos de Referencia

TicketAI no sólo permite la carga de Tickets, también permite la carga de "archivos de referencia".

Los Archivos de Referencia pueden interpretarse como "preventas", es decir, si se agendó con el cliente la entrega de un cierto paquete de artículos a surtir.

TicketAI esta diseñado para también leer este tipo de archivos, su generación y carga son muy importantes ya que, al tenerlos de referencia, se pueden conseguir "matches", en la sección de Documentos se detallará esta función.

#### Características de los archivos de Referencia

Los archivos de referencia deben tener el formato:
- .xls
- .xlxs

Los campos que debe tener el archivo de referencia y que harán match con los Tickets físicos escaneados son:

- Documentos

* Recepción
* Pedido
* Factura

-Cliente

* Nombre
* Sucursal

- Información de Transacción

* Entradas
* Salidas
* Precios
  
  # Buscar

Por su diseño, TicketAI permite la carga de muchos archivos, uno por cada Ticket, ante este volumen tan grande de información, se necesita un motor de búsqueda que este a la altura. 

TicketAI cuenta con un poderoso motor de búsqueda que permite identificar diferentes elementos que forman parte de los Tickets, por ejemplo:

- Productos
- Clientes
- Facturas

## Tipo de Búsquedas posibles

El motor de búsqueda con el que cuenta TicketAI permite realizar búsquedas cruzadas muy interesantes, combinando diferentes productos y clientes, a continuación, se muestran diferentes ejemplos de combinaciones:

- Producto 1, Producto 2, Producto 3 y tantos como sea posible. 
- Cliente 1, Cliente 2, Cliente 3 y tantos como sea posible.
- Cliente 1, Producto 1, Producto 2, Producto 3, y tantos productos como sea posible.
- Cliente 1, Cliente 2, Producto 1. 

## Flujo de Trabajo

![Buscar](https://user-images.githubusercontent.com/63880141/80723875-c61a6e00-8ac6-11ea-93c2-c8e0e75759b4.png)

### Precisiones Referentes al Flujo de Trabajo

Login: Acceso a la Plataforma

1.	Menú: El menú es el botón de la esquina superior izquierda.

2.	Buscar: Es una de las opciones que aparece en el menú desplegable.

3. Campo de Búsqueda: Este campo esta diseñado para aceptar "Etiqueta", se recomienda colocar una Etiqueta por Producto y/o Cliente. Para esto se debe escribir el nombre del producto o cliente y terminar con el botón "enter".

3.1 Si tecleó incorrectamente el nombre del Producto o Cliente, se puede dar clic en el "tachecito" de la Etiqueta, o bien, dar clic en el botón Limpiar.

3.2 Si tecleó todo correctamente dar clic en el botón buscar.

4. Aparece el listado de coincidencias.
 
4.1 Si se necesita obtener detalles de alguno de los Tickets mostrados, dar clic en el botón "Detalles". 
 
4.2 Si no encontró lo que buscaba, se puede ajustar la búsqueda en el paso 3.

## Detalles

Al dar clic en Detalles nos encontramos con una pantalla distinta con una gran variedad de opciones, para efectos de facilitar la explicación, en la sección "Documentos - Detalles" se da una revisión a Fondo de las acciones que aquí se pueden ejecutar.

# Documentos

TicketAI permite el almacenamiento de una gran cantidad de documentos, navegar entre esta información puede ser un poco retador, para facilitar la navegación, esta funcionalidad cuenta con un motor de consulta poderoso.


## Flujo Maestro

El motor de búsqueda que contiene esta funcionalidad cuenta con los siguientes filtros:

- Fechas: Se puede seleccionar un rango de fechas a consultar.
- Matches: Si se ingresó un documento de preventa que posteriormente es identificado con un ticket escaneado, se obtiene un "Match", en caso de no identificarlo, tendríamos un documento sin Match.

![Documentos_Maestro](https://user-images.githubusercontent.com/63880141/80723966-e2b6a600-8ac6-11ea-9860-064bb8634a00.png)

### Precisiones del Flujo

1. Se puede seleccionar el rango de fechas a filtrar, si no se desea filtrar por fechas, se omite este paso.
2. Tenemos la opción de seleccionar si la búsqueda incluirá o no Matches.
3. Con las preselecciones indicadas, el sistema mostrará la consulta indicada automáticamente.

## Tipos de Consultas

Teniendo en cuenta los filtros con los que contamos, podemos hacer los siguientes 4 tipos de consultas:

1. Consulta por Fechas y Documentos con Matches.
2. Consulta por Fechas y Documentos sin Matches.
3. Consulta sin Fechas y Documentos con Matches.
4. Consulta sin Fechas y Documentos sin Matches.

A continuación, se da una guía para conseguir cada uno de esos filtros.

### Consulta por Fechas y Documentos con Matches

El objetivo de esta consulta será identificar los documentos que tienen Match en un periodo de tiempo determinado.

![Fecha_con_Matches](https://user-images.githubusercontent.com/63880141/80724189-2c06f580-8ac7-11ea-8930-77e3ee852bfc.png)

#### Precisiones de este Flujo

Partiendo de la pantalla de inicio se debe:

1. Dar clic en el botón de la esquina superior izquierda.

2. Seleccionar la opción Documentos.

3. Dar clic en la opción de Rango de Fechas, esto desplegará un pequeño calendario, en ese calendario, debemos indicar el rango de fechas deseado.

4. Seleccionar la opción "Con Matches".

5. Esto desplegará el listado de coincidencias.

5.1 Si encuentra un documento particular que desee consultar para más información, dar clic en el botón Detalles.

5.2 Si no encuentra el documento buscado, se sugeriría ajustar la búsqueda.

6. Para ajustar la búsqueda retomaríamos las acciones desde el paso 3.

### Consulta por Fechas y Documentos sin Matches

En el caso de necesitar una consulta que nos permita identificar que documentos no tienen Match en un intervalo de tiempo determinado.

![Fecha_sin_Matches](https://user-images.githubusercontent.com/63880141/80724324-53f65900-8ac7-11ea-8ff5-f1fd27ef0f0b.png)

#### Precisiones de este Flujo

Partiendo de la pantalla de inicio se debe:

1. Dar clic en el botón de la esquina superior izquierda.

2. Seleccionar la opción Documentos.

3. Dar clic en la opción de Rango de Fechas, esto desplegará un pequeño calendario, en ese calendario, debemos indicar el rango de fechas deseado.

4. Seleccionar la opción "Sin Matches".

5. Esto desplegará el listado de coincidencias.

5.1 Si encuentra un documento particular que desee consultar para más información, dar clic en el botón Detalles.

5.2 Si no encuentra el documento buscado, se sugeriría ajustar la búsqueda.

6. Para ajustar la búsqueda retomaríamos las acciones desde el paso 3.

### Consulta sin Fechas y Documentos con Matches

En el supuesto de que no tengamos clara la fecha de algún ticket que necesitemos consultar, pero tengamos certidumbre de que aparece con un Match, se recomienda realizar esté tipo de consultas.

![Matches_sin_Fechas](https://user-images.githubusercontent.com/63880141/80724401-6a9cb000-8ac7-11ea-8bdb-4c36be0a0821.png)

#### Precisiones de este Flujo

Partiendo de la pantalla de inicio se debe:

1. Dar clic en el botón de la esquina superior izquierda.

2. Seleccionar la opción Documentos.

3. Seleccionar la opción "Con Matches".

4. Esto desplegará el listado de coincidencias.

5. Al encontrar el documento al que desee consultar, dar clic en Detalles.

### Consulta sin Fechas y Documentos sin Matches

En el supuesto de que no tengamos clara la fecha de algún ticket que necesitemos consultar, pero tengamos certidumbre de que tampoco aparece con un Match, se recomienda realizar este tipo de consulta.

![Sin_Matches_sin_Fechas](https://user-images.githubusercontent.com/63880141/80724490-8738e800-8ac7-11ea-96be-af66265b8483.png)

#### Precisiones de este Flujo

Partiendo de la pantalla de inicio se debe:

1. Dar clic en el botón de la esquina superior izquierda.

2. Seleccionar la opción Documentos.

3. Seleccionar la opción "Sin Matches".

4. Esto desplegará el listado de coincidencias.

5. Al encontrar el documento al que desee consultar, dar clic en Detalles.

# Detalles_Documento

Esta sección está diseñada para permitirnos visualizar los Tickets escaneados y su información. La información está clasificada de la siguiente forma:

1. Ticket. Se puede dar un clic en el Ticket para expandirlo.

2. Información. En este conjunto de contamos con los campos mostrados a continuación:

    2.1 Fecha del Archivo original.

    2.2 Fecha de Creación.

    2.3 Fecha de Modificación.

3. Documento. En este conjunto de contamos con los campos mostrados a continuación:

    3.1 Recepción.

    3.2 Pedido.

    3.3 Factura.

4. Cliente. En este conjunto de contamos con los campos mostrados a continuación:

   4.1 Nombre.

   4.2 Sucursal.

   4.3 Fecha.

   4.4 Proveedor.

   4.5 Hora de Entrada.

   4.6 Hora de Salida.

5. Información de Transacción. En este conjunto de contamos con los campos mostrados a continuación:

   5.1 Entradas. 

   5.2 Salidas. 

   5.3 C. Cargo. 

   5.4 Sub - Total.

   5.5 Descuento.

   5.6 Cargos.

   5.7 IEPS.

   5.8 IVA.

   5.9 Total.

   5.10 Total Calc.

6. Matches. En el caso de tener un documento con Matches, aparece el campo Coincidencias.

7. Detalles de Transacción. En este conjunto de contamos con los campos mostrados a continuación:

   7.1 Descripción.

   7.2 Cup.

   7.3 Entradas.

   7.4 Salidas.

   7.5 C/Cargos.

* Nota: Este campo contiene hasta 10 líneas de visualización por Default, se pueden ampliar a 15, todas o reducirse a 5. Si el documento incluye más artículos de los mostrados, se cuenta con flechas de navegación para visualizar el resto de los productos.

## Campo Coincidencias

Cuando un documento identifica un "Match" entre el Ticket y el documento de Pre-Venta Cargado, aparece el campo Coincidencias.

Este campo muestra la siguiente información:

a) Cliente.
b) Sucursal.
c) Fecha. 
d) Fecha de Expiración.
e) Número Cliente.
d) Número de Factura.
f) Valor de la Factura.
g) Descuento Acordado.
h) IVA.
i) IEPS. 
j) Total de la Factura.

La calidad General de la coincidencia se clasifica por un código alfanumerico:

A0  -  A1  -  A2  -  A3 
B0  -  B1  -  B2  -  B3 
C0  -  C1  -  C2  -  C3 
D0  -  D1  -  D2  -  D3 

Enfrente de los campos en los que tenga la coincidencia, aparece un icono con una letra:

A de color Verde: Coincidencia Optima.
B de color Amarillo: Buena calidad de Coincidencia.
C de color Naranja: Recomendable revisar este campo.
N/A de color Rojo: Altamente recomendable revisar estos detalles.

Es importante mencionar que en ocasiones los Tickets pueden tener algún sello, firma que TicketAI puede interpretar como un match de poca calidad, aunque la información sea correcta.

## Flujo de Trabajo

A continuación, se muestra el Flujo de Trabajo para Verificar coincidencias.

![Coincidencias](https://user-images.githubusercontent.com/63880141/80724572-9f106c00-8ac7-11ea-9a5c-81a69d14ddfd.png)

### Precisiones del Flujo de Trabajo

1. Clic en coincidencias: Esto nos permitirá identificar todos los campos con coincidencias.

2. Detallar Información: Si encontramos coincidencias con rangos C o menor es Altamente recomendable verificar.

2.1 En caso de que sea necesario detallar información, aplicar el Flujo de Editar Documentos.

2.2 Si desea revisar y verificar información voluntariamente, aplicar el Flujo de Editar Documentos.


## Flujo de Trabajo: Editar Documentos

Este flujo de trabajo da los detalles para editar información si es que fuera necesario.

![Flujo editar Documentos](https://user-images.githubusercontent.com/63880141/80724631-b18aa580-8ac7-11ea-8f59-17d4b46f6534.png)

### Precisiones Flujo de Trabajo: Editar Documentos

1. ¿Desea consultar información? Basado en las coincidencias, se recomienda revisar, por lo menos esos campos.

2. Si desea realizar cambios, dar clic en el campo editable.

3. Al verificar la información podremos saber si necesitamos ajustar algún detalle.

3.1 Si no necesita más detalles, ¿Consultará algún Campo más?.

4. En caso de necesitarlo, regresar a paso 2.

3.2 Si en necesario detallar algo, capturar el Detalle.

5. Verificar que la captura es correcta.

5.1 En caso de ser correcta, dar clic en "Guardar".

5.2 En caso de no estar satisfecho con la presión dar clic en "Cancelar".

6. Desea/ necesita detallar más información.

6.1 En caso de requerirlo, regresar a Paso 2.
