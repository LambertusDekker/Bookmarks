# Everything R

- https://cran.r-project.org/manuals.html
- https://cran.r-project.org/

'''R
library(odbc)

server_ <- "mydatabase.here.windows.net,1234"
database_ <- "DATABASNAME"
username_ <- "USERNAME"
password_ <- "PASSWORD"

con <- dbConnect(
    drv = odbc::odbc(),
    Driver = "SQL Server",
    server = server_,
    database = database_,
    uid = username_,
    pwd = password_
    )

sql_ <- "
SELECT [Col1]
      ,[Col2]
      ,[Col3]
FROM [dba].[Adresses]"

result_ <- dbGetQuery(con, sql_)
print(result_)
```
