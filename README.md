![]tools.png

# GEC
Gambas enhanced controls.
This is a collection of enhanced controls developed by some menbers of forum www.gambas-es.org.

## The enhanced controls

### dbcontrols
[Shordi]
Various controls for viewing databases

#### dbComboBox
[Shordi]
Displays a list of fields (listfields) of a sql query (sqlstring) of a declared connection (connection) and returns the value of a query field (fieldkey)

#### ListBox
[Shordi]
Lists the fields (listfields) of a sql query (sqlstring) of a declared connection and returns the value of a query field (fieldkey)
dbSqlTree
Create a tree with the fields (listfields) of a sql query (sqlstring) of a declared connection and return the value of a query field (fieldkey)
 
#### dbGrid
[Shordi]
List the result of a query sql (sqlstring) of a declared connection (connection) being able to choose the column that will have the return value (colkey). Provides the colkey content of the selected cells in the Array Value (Value). Allows you to set the column headings (titles), the widths of columns (widths).
Also sorts by clicking on the column headers.
First Click = ascending order
Second Click = descending order
Third Click = no order in column
Shift + Click = Cancel all orders and set only that ascending column

#### dbGridFilter
[Shordi]
It is a dbGrid that allows to set filters for the SQL query and Export the contents of the Grid to a .csv file
It also allows you to show or hide a button panel (showControls) and show or hide the default context menu (defaultmenu). It allows other contextual menus (Submenu) that can be added to the contextual menu or shown alone.

Note: To use them simply click on the button below and provide the carpet where a Gambas project resides. Then add to that project the shrimp components that use these controls:
gb.db
gb.form.mdi
gb.gui.qt.webkit
If our project does not use gb.gui.qt and uses gb.qt4 or gb.qt5 we should only bind instead of gb.gui.qt the gb.qt4 / qt5.webkit, necessary.

### htEdit
[Shordi]
Edit simple HTML. It allows text formatting and inclusion of links and images.

### xcontrols

#### filebox
[Shordi]
Select a file by pressing the db button

#### ProgressBarText
[Didier18]

#### TextBoxExplain
[Tobias]

#### TextList
[Roinnel]

#### ButtonSquare
[Jsbsan]


### Module Utilities
[Tincho]

#### ArrangePath
Devuelve una ruta sin los saltos del línea ni caracteres problemáticos requiere come parametro de entrada una ruta.

#### ArrayExclude
Quita de la lista los textos que tengan la cadena de texto pasada como parametro.

#### ArrayInclude
Quita de la lista los textos que NO tengan la cadena de texto pasada como parametro.

#### Capital
Devuelve un texto con la primera letra en mayusculas y todas las siguientes en minúsculas.

#### Chek4SQL
Devuelve un texto apto para consulatas SQL, quita los saltos del línea y los caracteres no compatibles con sentencias SQL.

#### ConvertPath
Devuelve una ruta con los caracteres hexadecimales decodificados en las URI's que se le pase.

#### CRC32
Obtencion del crc32 de un archivo del que se pasa como parametro la ruta completa, como parametro opcional strCase puede ser U o L que parara todo a Ucase o Lcase.

#### DirChooser
Selecciona la ruta de un directorio mediante una caja de dialogo.

#### FileChooser
Selecciona la ruta completa de un archivo, con el nombre y las extensión. Como opcional se puede pasar un directorio que es a donde se dirigira el filechooser cuando se abra.

#### FileExif
Devuelve una matriz con los datos extraídos por el programa de la terminal ExifTool.

#### FileInfo
Devuelve una matriz con datos del archivo que se le pasa como ruta.

#### FileNospace
Devuelve un texto, nombre de arcivo concatenando todos los fragmentos que se le pase y pone todo en minusculas quita los caracteres fuera del rango 97-122 de ascci.

#### FileVersion
Devuelve un texto con la versión del archivo que se le pasa como ruta. Usa el comando file de la terminal.

#### HMStoSeconds
Devuelve el tiempo en segundos de una cadena que se le pase con el formato HH:MM:SS HORAS:MINUTOS:SEGUNDOS.

#### ListDeldup
Elimina elementos duplicados de una lista, requiere una String[] y devuelve una String[].

#### MkConfXml
Creacion de archivo de configuracion inicial xml.

#### MouseButton
Funcion que retorna el nombre en ingés del boton del ratón que se ha presionado.

#### NamingCon
Devuelve una lista de nombres de controles y su abreviación de tres caracteres.

#### ScanFolder
Escanea una carpeta que se pasa como parametro en busca de archivos se puede filtrar con una lista de extensiones separadas por comas.

#### Timestamp
Retorna una cadena de texto con el tiempo en formato "yyyymmddhhnnss".

#### WhereRun
Devuelve si el programa gambas se esta ejecutando desde el IDE o desde un .gambas.
