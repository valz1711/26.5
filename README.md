# 26.5
Types of table
Managed table:
Managed table is also called as Internal table. This is the default table in Hive. When we create a table in Hive without specifying it as external, by default we will get a Managed table. If we create a table as a managed table, the table will be created in a specific location in HDFS.
  By default, the table data will be created in /usr/hive/warehouse directory of HDFS. If we delete a Managed table, both the table data and meta data for that table will be deleted from the HDFS.
  
External table:
External table is created for external use as when the data is used outside Hive. Whenever we want to delete the table’s meta data and we want to keep the table’s data as it is, we use External table. External table only deletes the schema of the table. Hive should not own data and control settings, dirs, etc., you have another program or process that will do those things. 
