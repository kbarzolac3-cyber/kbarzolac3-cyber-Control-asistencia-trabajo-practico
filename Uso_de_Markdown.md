# Investigación sobre Markdown

## [cite_start]1. ¿Qué es Markdown y por qué se utiliza? [cite: 268]
Markdown es un lenguaje de marcado ligero creado por John Gruber en 2004. Su objetivo es permitir a las personas escribir usando un formato de texto plano fácil de leer y fácil de escribir, que luego se convierte de manera opcional a HTML (o PDF, u otros formatos) estructuralmente válido.

Se utiliza masivamente en proyectos de software (especialmente en archivos `README.md`) porque permite a los desarrolladores:
* Crear documentación de forma rápida y sencilla sin usar software complicado como Word.
* Escribir texto formateado (listas, negritas, enlaces) directamente en el código.
* Asegurar que la documentación sea legible tanto en su forma "cruda" (texto plano) como en su forma "renderizada" (en GitHub, por ejemplo).

## [cite_start]2. Ejemplo práctico de uso de Markdown [cite: 269]

![logo](https://upload.wikimedia.org/wikipedia/commons/thumb/8/80/Wikipedia-logo-v2.svg/1200px-Wikipedia-logo-v2.svg.png)


* Elemento 1
* Elemento 2
    * Un sub-elemento
  
| Columna 1 | Columna 2 |
|:----------|-----------|
| Dato A    | Dato B    |
| Dato C    | Dato D    |


### Encabezados
```markdown
# Encabezado Nivel 1
## Encabezado Nivel 2
### Encabezado Nivel 3
* Elemento 1
* Elemento 2
    * Sub-elemento 2.1
1.  Elemento ordenado 1
2.  Elemento ordenado 2

| Columna 1 | Columna 2 |
|  ---------| --------- |
| Celda 1. | Celda 1.|
| Celda 2. | Celda 2. |

* Elemento 1
* Elemento 2
    * Un sub-elemento
| Columna 1 | Columna 2 |
|-----------|-----------|
| Dato A    | Dato B    |
| Dato C    | Dato D    |

![logo de Wikipedia](https://upload.wikimedia.org/wikipedia/commons/thumb/8/80/Wikipedia-logo-v2.svg/1200px-Wikipedia-logo-v2.svg.png)
