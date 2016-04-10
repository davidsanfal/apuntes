# Apuntes de SQL

Crea una tabla definiendo su nombre y sus columnas con su tipo.
```sql
CREATE TABLE table_name (column_1_name data_type, column_2_name data_type, ...);
```
Crea una fila nueva definiendo los valores que toman cada una de sus columnas.
```sql
INSERT table_name (column_1_name, column_2_name, ...) VALUES (1, 'hola', ...);
```
Retorna todas las filas de una tabla.
```sql
SELECT * FROM table_name;
```
retorna todos los valores de una columna de una tabla.
```sql
SELECT column_name FROM table_name;
```
retorna todos los valores de varias columnas de una tabla.
```sql
SELECT column_3_name, column_1_name FROM table_name;
```
Actualiza el valor de asociado a una columna de las filas donde tengan un valor determinado en otra columna (o en la misma).
Ej. Cambia el valor de la column_2_name a 22 en todas las filas que tengan un valor de 1 en su column_1_name.
```sql
UPDATE table_name SET column_2_name = 22 WHERE column_1_name = 1;
```
Añade una columna nueva a una tabla existente.
```sql
ALTER TABLE table_name ADD COLUMN new_column_name data_type;
```
Elimina todas las filas que tengan un valor determinado en una columna.
Ej, Elimina todas las filas que tengan un valor NULL (no tengan ningun valor) en la column_7_name.
```sql
DELETE FROM table_name WHERE column_7 IS NULL;
```
Retorna los distintos valores de una columna sin repetir.
Ej, saber todas las categorías que tiene una base de datos de libros.
```sql
SELECT DISTINCT column_name FROM table_name;
```

...(EN PROCESO)...
