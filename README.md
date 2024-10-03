This repository documents the steps involved in creating and deleting a Pluggable Database (PDB) in Oracle Database.
It also includes screenshots of the Oracle Enterprise Manager dashboard, demonstrating key tasks related to PDB management.

queries used in this work
 DELETING QUERY OF PDB
 
 sql> alter pluggable database pdb5 unplug into'C:\app\kezal\product\21c\admin\xe\dpdump\hr.xml';

  CREATING  QUERY OF PDB

  
 sql> CREATE PLUGGABLE DATABASE PDB3
  2  ADMIN USER PDBACE IDENTIFIED BY ACE
  3  FILE_NAME_CONVERT = ('C:\APP\KEZA\PRODUCT\21C\ORADATA\XE\PDBSEED\','C:\APP\KEZA\PRODUCT\21C\ORADATA\XE\XEPDB1\PDB3\');

MANAGER DASHBOARD

  sql> select dbms_xdb_config.gethttpsport() from dual;
