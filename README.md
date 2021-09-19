# DBeaver-Driver-All
```bash
____________                            ______      _                    
|  _  \ ___ \                           |  _  \    (_)                   
| | | | |_/ / ___  __ ___   _____ _ __  | | | |_ __ ___   _____ _ __ ___ 
| | | | ___ \/ _ \/ _` \ \ / / _ \ '__| | | | | '__| \ \ / / _ \ '__/ __|
| |/ /| |_/ /  __/ (_| |\ V /  __/ |    | |/ /| |  | |\ V /  __/ |  \__ \
|___/ \____/ \___|\__,_| \_/ \___|_|    |___/ |_|  |_| \_/ \___|_|  |___/
```
`DBeaver-Driver-All` ( `DBeaver驱动包` )整合所有DBeaver的JDBC驱动包，供DBeaver使用，无需每次都搜索和下载，只需clone本项目即可，一个包包含几乎所有的驱动，如果有缺漏的驱动欢迎提Issue补充。

>`DBeaver-Driver-All`, a `DBeaver JDBC Driver Package` , contains all jdbc drivers for dbeaver,no need to download it everytime ,all drivers in one package .

# Author
Powered by Moshow郑锴@[zhengkai.blog.csdn.net](http://zhengkai.blog.csdn.net)

# Version
Dbeaver : `21.2` 

# 包含JDBC驱动列表(jdbc driver list)
- athena-jdbc-custom-credentials-provider-0.0.1-SNAPSHOT.jar
- AthenaJDBC42-2.0.16.1000.jar
- CacheDB.jar
- checker-qual-2.11.1.jar
- clickhouse-jdbc-0.2.4.jar
- clickhouse-jdbc-0.2.6.jar
- commons-codec-1.11.jar
- commons-codec-1.9.jar
- commons-logging-1.2.jar
- error_prone_annotations-2.3.4.jar
- failureaccess-1.0.1.jar
- guava-19.0.jar
- guava-29.0-jre.jar
- httpclient-4.5.13.jar
- httpclient-4.5.2.jar
- httpcore-4.4.13.jar
- httpcore-4.4.4.jar
- httpmime-4.5.13.jar
- httpmime-4.5.2.jar
- j2objc-annotations-1.3.jar
- jackson-annotations-2.7.0.jar
- jackson-annotations-2.9.10.jar
- jackson-core-2.7.3.jar
- jackson-core-2.9.10.jar
- jackson-databind-2.7.3.jar
- jackson-databind-2.9.10.8.jar
- javax.activation-api-1.2.0.jar
- jaxb-api-2.3.0.jar
- jsr305-3.0.2.jar
- listenablefuture-9999.0-empty-to-avoid-conflict-with-guava.jar
- lz4-1.3.0.jar
- slf4j-api-1.7.21.jar
- slf4j-api-1.7.30.jar
- csvjdbc-1.0.35.jar
- csvjdbc-1.0.37.jar
- dans-dbf-lib-1.0.0-beta-10.jar
- db2jcc4.jar
- jt400.jar
- derby-10.15.1.3.jar
- derbyclient-10.15.1.3.jar
- derbyshared-10.15.1.3.jar
- derbytools-10.15.1.3.jar
- exasol-jdbc-6.1.0.jar
- h2-1.4.196.jar
- ngdbc-2.5.49.jar
- hive-jdbc-uber-2.6.5.0-292.jar
- hsqldb-2.4.0.jar
- ifxjdbc.jar
- ifxlang.jar
- jdbc-4.50.4.1.jar
- iijdbc.jar
- antlr4-runtime-4.7.2.jar
- connector-api-1.5.jar
- jaybird-4.0.0.java8.jar
- jtds-1.3.1.jar
- mariadb-java-client-2.6.0.jar
- mariadb-java-client-2.7.1.jar
- sapdbc-7.6.06.jar
- mssql-jdbc-8.2.0.jre8.jar
- mssql-jdbc-9.2.0.jre8.jar
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
- postgis-geometry-2.5.0.jar
- postgis-jdbc-2.2.1.jar
- postgis-jdbc-2.5.0.jar
- postgis-jdbc-jtsparser-2.5.0.jar
- postgresql-42.2.20.jar
- postgresql-42.2.5.jar
- aws-java-sdk-core-1.11.118.jar
- aws-java-sdk-redshift-1.11.118.jar
- aws-java-sdk-sts-1.11.118.jar
- commons-codec-1.9.jar
- commons-logging-1.1.3.jar
- httpclient-4.5.2.jar
- httpcore-4.4.4.jar
- jackson-annotations-2.10.1.jar
- jackson-core-2.10.1.jar
- jackson-databind-2.10.1.jar
- jackson-dataformat-cbor-2.10.1.jar
- joda-time-2.8.1.jar
- log4j-1.2.17.jar
- RedshiftJDBC42-no-awssdk-1.2.45.1069.jar
- RedshiftJDBC42-no-awssdk-1.2.47.1071.jar
- sqlite-jdbc-3.30.1.jar
- jconn3.jar
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


# PowerShell输出所有jar文件名
to output all jar list in folder
```bash
#输出所有jar文件的文件名
Get-ChildItem "D:\workspace\jar\dbeaver-driver-all\drivers" -Include *.jar -Recurse -Force| ForEach-Object -Process{
    if($_ -is [System.IO.FileInfo])
    {
        Write-Host "-" $_.Name
    }
}
```

#Update Log
|更新时间|版本|
|----|----|
|2021-09-19|update to 21.2|
|2020-10-18|update to 7.2.0|
|2020-07-09|update to 7.1.0|
