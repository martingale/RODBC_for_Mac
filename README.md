# RODBC_for_Mac

To setup a MS SQL driver in Mac OS first, install freetds with unixodbc arguement

`brew install freetds --with-unixodbc`

Create the file ~/Library/ODBC/odbc.ini 

`vi ~/Library/ODBC/odbc.ini`

and fill the file with with the following chunk: 
~~~
[osmanli]
Description =Osmanli Bond Veritabani
TDS_Version = 7.2
Driver = /usr/local/lib/libtdsodbc.so
Server = 212.15.8.153
Setup=/usr/local/lib/libtdsodbc.so
Port = 1433
~~
Copy ~/Library/ODBC/odbc.ini also to /usr/local/Cellar/unixodbc/2.3.4/etc/odbc.ini
`cp ~/Library/ODBC/odbc.ini /usr/local/Cellar/unixodbc/2.3.4/etc/odbc.ini`

`install.packages("RODBC")`

