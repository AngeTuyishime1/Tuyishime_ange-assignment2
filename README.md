# Tuyishime_ange-assignment2
SQL> CREATE PLUGGABLE DATABASE plsql_class2024db
  2   ADMIN USER an_plsplauca IDENTIFIED BY ange123
  3  FILE_NAME_CONVERT = ('C:\oracle21c\oradata\ORCL\pdbseed',
  4                     'C:\oracle21c\oradata\ORCL\pdbseed\sqlplus\pdbs\an_plsqlauca');

Pluggable database created.
--this SQL command creates a new pluggable database named plsql_class2024db, sets up an administrative user with specified credentials, and defines where the database files will be located.

SQL> ALTER PLUGGABLE DATABASE an_to_delete_pdb CLOSE IMMEDIATE;

--the command ALTER PLUGGABLE DATABASE an_to_delete_pdb CLOSE IMMEDIATE; is used to immediately close the pluggable database named an_to_delete_pdb, making it unavailable for any further connections or transactions. 

SQL> ALTER PLUGGABLE DATABASE an_to_delete_pdb UNPLUG INTO 'C:\oracle21c\oradata\ORCL\pdbseed\sqlplus\pdbs\de_plsqlauca\an_to_delete_pdb.xml';

the command ALTER PLUGGABLE DATABASE an_to_delete_pdb UNPLUG INTO 'C:\oracle21c\oradata\ORCL\pdbseed\sqlplus\pdbs\de_plsqlauca\an_to_delete_pdb.xml'; is used to unplug the pluggable database named an_to_delete_pdb and save its metadata to the specified XML file. 
