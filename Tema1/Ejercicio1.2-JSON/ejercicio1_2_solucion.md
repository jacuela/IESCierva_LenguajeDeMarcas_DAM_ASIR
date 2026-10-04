Autor: Juan Antonio Cuello\
Clase: 1º DAM  

---

# EJERCICIO 1.2 - PRACTICANDO CON JSON

# Tarea1
```json
{
"titulo": "El señor de los anillos",
"genero": "Fantasia",
"anio": 1954,
"disponible": true
}
```

Tipos: titulo → texto; genero → texto; anio → número; disponible → booleano.


# Tarea2
```json
{
"titulo": "El señor de los anillos",
"genero": "Fantasia",
"anio": 1954,
"disponible": true,
"autor": "J. R. R. Tolkien",
"paginas": 1178,
"editorial": "Minotauro"
}
```

1178 es un número; "1178" es texto (string).


# Tarea3
```json
{
"titulo": "El señor de los anillos",
"generos": ["Fantasia", "Aventura", "Accion"],
"anio": 1954,
"disponible": true,
"autor": "J. R. R. Tolkien",
"paginas": 1178,
"editorial": "Minotauro"
}
```

Una propiedad de texto contiene un único valor textual; un array permite almacenar una colección
ordenada de valores.


# Tarea4
```json
{
    "titulo": "El señor de los anillos",
    "autor": {
        "nombre": "J. R. R.",
        "apellido": "Tolkien",
        "nacionalidad": "Britanica"
    },
    "editorial": {
        "nombre": "Minotauro",
        "pais": "España"
    }
}
``` 
- Nombre de la editorial: data.editorial.nombre
- Título del libro: data.titulo
- Nombre del autor: data.autor.nombre



# Tarea5
```json
{
	"libros": [
		{
            "titulo": "El señor de los anillos", 
            "genero": "Fantasia", 
            "anio": 1954
        },
		{
            "titulo": "Harry Potter y la piedra filosofal", 
            "genero": "Fantasia", 
            "anio": 1997
        },
		{
            "titulo": "1984", 
            "genero": "Ciencia ficcion", 
            "anio": 1949
        }
	]
}
``` 

El array está asociado a libros; contiene 3 objetos. 
- El título del primer libro: data.libros[0].titulo
- El título del tercer libro: data.libros[2].titulo
- Genero del segundo libro: data.libros[1].genero
 


# Tarea6

```json
Hay tres errores: una coma después de "Accion" antes de cerrar el array, la llave _autor_ debe ir entre comillas dobles y True debe escribirse true. JSON distingue entre mayúsculas y minúsculas.

{
	"titulo": "El señor de los anillos",
	"autor": "Tolkien",
	"anio": 1954,
	"generos": ["Fantasia", "Aventura", "Accion"],
	"disponible": true
}

```

---

```json
Solucion al segundo JSON:
[
  {
    "nombre": "Juan",
    "edad": 18,
    "email": "juan@kk.com",
    "direccion": {
      "calle": "una calle",
      "numero": 2,
      "codigopostal": 30007
    }
  },
  {
    "nombre": "Pepe",
    "edad": 24,
    "email": "pepe@kk.com",
    "direccion": {
      "calle": "una calle",
      "numero": 2,
      "codigopostal": 30007
    }
  }
]
```

- El email de la primera persona de la lista: data[0].email
- La calle de la segunda persona de la lista: data[1].direccion.calle



# Tarea7
```json
{
    "libro": {
        "titulo": "El señor de los anillos",
        "genero": "Fantasia",
        "anio": 1954
    }
}
```

```json
{
    "alumno": {
        "nombre": "Ana",
        "edad": 20,
        "ciclo": "DAM",
        "activo": true
    }
}
```

# Tarea8

```json
{
  "biblioteca": {
    "nombre": "Biblioteca Municipal",
    "direccion": "Calle Mayor 10",
    "libros": [
      {
        "titulo": "Dune",
        "anio": 1965,
        "genero": "Ciencia ficcion",
        "paginas": 688,
        "disponible": true,
        "autor": {
          "nombre": "Frank Herbert",
          "nacionalidad": "Estadounidense"
        }
      },
      {
        "titulo": "1984",
        "anio": 1949,
        "genero": "Ciencia ficcion",
        "paginas": 328,
        "disponible": false,
        "autor": {
          "nombre": "George Orwell",
          "nacionalidad": "Britanica"
        }
      },
      {
        "titulo": "El Hobbit",
        "anio": 1937,
        "genero": "Fantasia",
        "paginas": 310,
        "disponible": true,
        "autor": {
          "nombre": "J. R. R. Tolkien",
          "nacionalidad": "Britanica"
        }
      }
    ]
  }
}

```


# Tarea9
```json
{
  "biblioteca": {
    "nombre": "Biblioteca Municipal",
    "direccion": "Calle Mayor 10",
    "libros": [
      {
        "titulo": "Dune",
        "anio": 1965,
        "genero": "Ciencia ficcion",
        "paginas": 688,
        "disponible": true,
        "autor": {
          "nombre": "Frank Herbert",
          "nacionalidad": "Estadounidense"
        }
      },
      {
        "titulo": "1984",
        "anio": 1949,
        "genero": "Ciencia ficcion",
        "paginas": 328,
        "disponible": false,
        "autor": {
          "nombre": "George Orwell",
          "nacionalidad": "Britanica"
        }
      }
    ]
  }
}

- Nombre de la biblioteca: data.biblioteca.nombre
- Título del primer libro: data.biblioteca.libros[0].titulo
- Título del segundo libro: data.biblioteca.libros[1].titulo
- Nombre del autor del segundo libro: data.biblioteca.libros[1].autor.nombre
- ¿Está disponible el primer libro?: data.biblioteca.libros[0].disponible


```

