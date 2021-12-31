# M06C03 
## Trabajo individual entregable de base de datos

> Base de datos relacional uno a muchos, muchos a uno y muchos a muchos
> Diagrama de flujos
> Ejemplo de consulta relacionando todas las tablas


### Ejemplo de consulta

```SQL
SELECT usuarios.Nombre, categorias.Categoria, notas.titulo AS Titulo, notas.descripcion AS Descripción 
FROM notascategorias
INNER JOIN categorias ON notascategorias.idCategorias = categorias.id
INNER JOIN notas ON notascategorias.idNotas = notas.id
INNER JOIN usuarios ON notas.id = usuarios.idNotas
```

![](https://github.com/Nacho261013/M0C03/blob/main/M06C03/Consulta.jpg)

### Links

> [Imagen de diagrama de flujos](https://github.com/Nacho261013/M0C03/blob/main/M06C03/DiagramaDB.jpg)
> [HTML de diagrama de flujos](https://github.com/Nacho261013/M0C03/blob/main/M06C03/M06C03%20Entregable.html)
=



