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
input: strPathRaw As String
Return: String

#### ArrayExclude
(stxList As String[], strFind As String) As String[]

#### ArrayInclude
(stxList As String[], strFind As String) As String[]

#### Capital
(strInput As String) As String

#### Chek4SQL
(strInput As String) As String

#### ConvertPath
(txt As String) As String

#### CRC32
(stInputPath As String, Optional strCase As String) As String
Obtencion del crc32 de un archivo del que se pasa como parametro la ruta completa, como parametro opcional strCase puede ser U o L que parara todo a Ucase o Lcase.

#### DirChooser
(Optional stInputPath As String) As String

#### ExifTool
(strPath As String) As String[]

#### FileChooser
(Optional strInputPath As String, Optional strFilter As String) As String
Selecciona la ruta completa de un archivo, con el nombre y las extensión. Como opcional se puede pasar un directorio que es a donde se dirigira el filechooser cuando se abra.

#### FileInfo
(strFilePath As String) As String[]

#### FileNospace
(stxParam As String[], Optional strDelim As String, Optional strExt As String) As String
Devuelve un texto, nombre de arcivo concatenando todos los fragmentos que se le pase y pone todo en minusculas quita los caracteres fuera del rango 97-122 de ascci

#### FileTemplate
(strFileSeed As String, strFileProduct As String, stxTag As String[], stxDat As String[])
Toma un archivo template xml y le reemplaza los tags por valores. el metodo sirve para hacer cualquier tipo dedocumento en pdf basandose claro esta en un archivo.dia

#### FileVersion
(strInputPath As String) As String
Devuelve la version del archivo que se le pase

#### HMStoSeconds
(strTime As String) As Integer

#### ImageStatTemp
(strPath As String) As String[]
Devuelve datos de la imagen que se le pase. de momento solo Ancho y Alto.

#### ListDeldup
(stxInput As String[]) As String[]

#### MkConfXml
(strXmlPath As String) As Integer
Creacion de archivo de configuracion inicial xml

#### MouseButton
(intKey As Integer) As String
Funcion que retorna el nombre en ingés del boton del ratón que se ha presionado.

#### NamingCon
() As String[]
Devuelve una lista de nombres de controles y su abreviación de tres caracteres

#### Timestamp
(datTime As Date) As String
Retorna una cadena de texto con el tiempo en formato "yyyymmddhhnnss"

#### TypeVar
(intType As Integer) As String
Función que devuelve el tipo de variable como una palabra. Como parametro de entrada requiere un numero entero.

#### Werun
(strProc1 As String) As Integer
Devuelve si el programa se ejecuta desde el ide o no

#### Notify
(strTitle As String, strBody As String)
Envia una notificacion al escritorio

#### ScanFolder
(strDir As String, Optional strExt As String) As String[]
Escanea una carpeta que se pasa como parametro en busca de archivos se puede filtrar con una lista de extensiones separadas por comas.

#### SendEmail
(stxAddreses As String[], stxNames As String[], Optional strMode As String, Optional strSubject As String, Optional strBody As String, Optional strAttachment As String)
Prepara los datos de un email y abre el programa por defecto para presentarlo.
