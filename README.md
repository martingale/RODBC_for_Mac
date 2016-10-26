# RODBC_for_Mac

First, install freetds with unixodbc arguement

`brew install freetds --with-unixodbc`

Create the file ~/Library/ODBC/odbc.ini 

`vi ~/Library/ODBC/odbc.ini`

and fill it with 

`[osmanli]
Description =Osmanli Bond Veritabani
TDS_Version = 7.2
Driver = /usr/local/lib/libtdsodbc.so
Server = 212.15.8.153
Setup=/usr/local/lib/libtdsodbc.so
Port = 1433`


`install.packages("RODBC")`
