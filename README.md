# DBeaver-Driver-All
`DBeaver-Driver-All` ( `DBeaver驱动包` )整合所有DBeaver的JDBC驱动包，供DBeaver使用，无需每次都搜索和下载，只需clone本项目即可，一个包包含几乎所有的驱动，如果有缺漏的驱动欢迎提Issue补充。

>`DBeaver-Driver-All`, a `DBeaver JDBC Driver Package` , contains all jdbc drivers for dbeaver,no need to download it everytime ,all drivers in one package .

# Author
Powered by Moshow郑锴@[zhengkai.blog.csdn.net](zhengkai.blog.csdn.net)

# Version
Dbeaver:`7.1.0`

# 包含JDBC驱动列表(jdbc driver list)
- CacheDB.jar
- clickhouse-jdbc-0.2.4.jar
- commons-codec-1.9.jar
- commons-logging-1.2.jar
- guava-19.0.jar
- httpclient-4.5.2.jar
- httpcore-4.4.4.jar
- httpmime-4.5.2.jar
- jackson-annotations-2.7.0.jar
- jackson-core-2.7.3.jar
- jackson-databind-2.7.3.jar
- jaxb-api-2.3.0.jar
- lz4-1.3.0.jar
- slf4j-api-1.7.21.jar
- csvjdbc-1.0.35.jar
- dans-dbf-lib-1.0.0-beta-10.jar
- db2jcc4.jar
- jt400.jar
- derby-10.15.1.3.jar
- derbyclient-10.15.1.3.jar
- derbyshared-10.15.1.3.jar
- derbytools-10.15.1.3.jar
- exasol-jdbc-6.1.0.jar
- h2-1.4.196.jar
- hive-jdbc-uber-2.6.5.0-292.jar
- hsqldb-2.4.0.jar
- ifxjdbc.jar
- ifxlang.jar
- iijdbc.jar
- antlr4-runtime-4.7.2.jar
- connector-api-1.5.jar
- jaybird-4.0.0.java8.jar
- jtds-1.3.1.jar
- mariadb-java-client-2.6.0.jar
- sapdbc-7.6.06.jar
- mssql-jdbc-8.2.0.jre8.jar
- mysql-connector-java-5.1.48.jar
- mysql-connector-java-8.0.17.jar
- protobuf-java-3.6.1.jar
- nzjdbc3.jar
- jdbc-odbc-bridge-jre7.jar
- ojdbc8.jar
- oraclepki.jar
- orai18n.jar
- osdt_cert.jar
- osdt_core.jar
- xdb6.jar
- xmlparserv2.jar
- postgis-jdbc-2.2.1.jar
- postgresql-42.2.5.jar
- sqlite-jdbc-3.30.1.jar
- jconn4.jar
- tdgssconfig.jar
- terajdbc4.jar
- byte-buddy-1.6.11.jar
- byte-buddy-agent-1.6.11.jar
- commons-lang-2.6.jar
- commons-logging-1.1.3.jar
- hsqldb-2.3.1.jar
- jackcess-2.1.6.jar
- mockito-core-2.7.22.jar
- objenesis-2.5.jar
- ucanaccess-4.0.2.jar
- vertica-jdbc-8.1.1-5.jar
- caffeine-2.6.2.jar
- waffle-jna-1.9.0.jar


# PowerShell输出所有jar文件名
to output all jar list in folder
```bash
#输出所有jar文件的文件名
Get-ChildItem "D:\workspace\java\dbeaver-driver-all\drivers" -Include *.jar -Recurse -Force| ForEach-Object -Process{
    if($_ -is [System.IO.FileInfo])
    {
        Write-Host $_.Name　
    }
}
```