# GDD-Migration-and-BI

This is a group project for the subject "Data Management" in UTN FRBA.
Teammates:

- Abril Caruso
- Guadalupe Fernández
- Tomás Gómez

For this project, a master single-table was given as an initial point. The goal was to design a new database schema with good practices like normalization and de-normalization when necessary (DER.jpg), a migration script to take data from the old to the new schema (data/script_creacion_inicial.sql), and a Business Intelligence schema (DER_BI.jpg) for which a migration script and views were created (data/script_creacion_bi.sql).

The BI Model follows a Star - Data Warehouse model as it is seen in the DER_BI.jpg.

## How to run the migrations:
Note: I recommend using Microsoft SQL Server 2012, which was the DBMS used for the project.

1. Decompress master-data/gd_esquema.Maestra.Table.rar
2. Run master-data/EjecutarScriptTablaMaestra.bat, you can tweak the command as you like to match your DBMS configurations. This will take a while, please be patient.
3. Run data/script_creacion_inicial.sql
4. Run data/script_creacion_BI.sql
5. Now, both the operational and BI models should be created in the database, under the BLACKSUITS schema.
