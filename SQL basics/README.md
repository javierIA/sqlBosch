

# Proyecto Infonavit

Este proyecto consiste en administrar los datos de la tabla "infonavit". Aquí proporcionamos ejemplos de cómo realizar operaciones CRUD (Crear, Leer, Actualizar, Borrar) en SQL.

## Crear (INSERT INTO)

Para agregar nuevos registros a la tabla:

```sql
INSERT INTO [dbo].[infonavit] 
(ano, mes, cve_ent, entidad, cve_mun, municipio, organismo, modalidad, destino, tipo, sexo, edad_rango, ingresos_rango, vivienda_valor, acciones, monto) 
VALUES 
(2023, 7, 1, 'Entidad1', 1001, 'Municipio1', 1, 1, 1, 1, 1, 1, 1, 1, 100.00, 200000.00)
```

## Leer (SELECT)

Para leer (o seleccionar) registros de la tabla:

```sql
SELECT * FROM [dbo].[infonavit]
```

## Actualizar (UPDATE)

Para actualizar registros existentes en la tabla:

```sql
UPDATE [dbo].[infonavit]
SET monto = 300000.00
WHERE ano = 2023 AND mes = 7 AND entidad = 'Entidad1'
```

## Borrar (DELETE)

Para eliminar registros de la tabla:

```sql
DELETE FROM [dbo].[infonavit]
WHERE ano = 2023 AND mes = 7 AND entidad = 'Entidad1'
```

**Nota:** Por favor, ten cuidado al utilizar el comando `DELETE`, ya que los datos borrados no se pueden recuperar.

---

Azure Data Studio por defecto sólo muestra las primeras 5000 filas de un resultado de consulta. Si deseas aumentar este límite, puedes seguir los siguientes pasos:

Haz clic en "File" en la barra de menú superior.
Luego, elige "Preferences".
Selecciona "Settings".
En el cuadro de búsqueda que aparece, escribe "SQL Editor: Max Rows".
Modifica la configuración "SQL Editor: Max Rows" a la cantidad que prefieras. Por ejemplo, si deseas que se muestren hasta 100000 filas, puedes cambiar este valor a 100000.
Presiona "Enter" y cierra la ventana de configuración.

 ---
