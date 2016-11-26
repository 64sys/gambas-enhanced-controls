# GEC
Gambas enhanced controls.
This is a collection of enhanced controls developed by some menbers of forum www.gambas-es.org.

## The enhanced controls

### dbcontrols [Shordi]
Various controls for viewing databases

#### dbComboBox [Shordi]
Displays a list of fields (listfields) of a sql query (sqlstring) of a declared connection (connection) and returns the value of a query field (fieldkey)

#### ListBox [Shordi]
Lists the fields (listfields) of a sql query (sqlstring) of a declared connection and returns the value of a query field (fieldkey)
dbSqlTree
Create a tree with the fields (listfields) of a sql query (sqlstring) of a declared connection and return the value of a query field (fieldkey)
 
#### dbGrid [Shordi]
List the result of a query sql (sqlstring) of a declared connection (connection) being able to choose the column that will have the return value (colkey). Provides the colkey content of the selected cells in the Array Value (Value). Allows you to set the column headings (titles), the widths of columns (widths).
Also sorts by clicking on the column headers.
First Click = ascending order
Second Click = descending order
Third Click = no order in column
Shift + Click = Cancel all orders and set only that ascending column

#### dbGridFilter [Shordi]
It is a dbGrid that allows to set filters for the SQL query and Export the contents of the Grid to a .csv file
It also allows you to show or hide a button panel (showControls) and show or hide the default context menu (defaultmenu). It allows other contextual menus (Submenu) that can be added to the contextual menu or shown alone.

Note: To use them simply click on the button below and provide the carpet where a Gambas project resides. Then add to that project the shrimp components that use these controls:
gb.db
gb.form.mdi
gb.gui.qt.webkit
If our project does not use gb.gui.qt and uses gb.qt4 or gb.qt5 we should only bind instead of gb.gui.qt the gb.qt4 / qt5.webkit, necessary.

### htEdit [Shordi]
Edit simple HTML. It allows text formatting and inclusion of links and images.

### xcontrols

#### filebox [Shordi]
Select a file by pressing the db button

#### ProgressBarText [Didier18]

#### TextBoxExplain [Tobias] 

#### TextList [Roinnel]

#### ButtonSquare [Jsbsan]

