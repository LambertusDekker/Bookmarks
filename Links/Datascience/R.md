# R Docs

-   [R project](https://cran.r-project.org/)
-   [R Manuals](https://cran.r-project.org/manuals.html)
-   [R for Datascience](https://r4ds.hadley.nz)

## SQL connection with R
```r
library(odbc)

server_ <- "mydatabase.here.windows.net,1234"
database_ <- "DATABASNAME"
username_ <- "USERNAME"
password_ <- "PASSWORD"

# Connecting
con <- dbConnect(
    drv = odbc::odbc(),
    Driver = "SQL Server",
    server = server_,
    database = database_,
    uid = username_,
    pwd = password_
    )

# SQL statement
sql_ <- "
SELECT [Col1]
      ,[Col2]
      ,[Col3]
FROM [dba].[Adresses]"

# running the whole thing
result_ <- dbGetQuery(con, sql_)
print(result_)
```
