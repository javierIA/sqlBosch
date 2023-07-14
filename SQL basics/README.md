

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

