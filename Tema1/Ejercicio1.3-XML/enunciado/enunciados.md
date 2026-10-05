Autor: Juan Antonio Cuello\
Clase: 1º DAM / ASIR 

---

# ENUNCIADOS SINTAXIS XML

## Ejercicio01
Crear un XML para describir una persona con sexo, nombre y apellidos. 

## Ejercicio02
Crear un XML con una lista de dos clientes. Cada cliente tienen nombre y cif. 

## Ejercicio03
Corregir los errores del siguiente XML

```xml
<?xml version="1.0" encoding="UTF-8" ?>
<nota fecha=12/11/99>
  <para>Elisa</para>
  <de>Pedro<de>
  <titulo>Recordatorio</titulo>
  <cuerpo>No olvides nuestra cita!
</notas>
```

## Ejercicio04
Crear un XML para representar el "personal" de una empresa. Estará formado por una lista de "personas". Cada persona tendrá nombre, email, direccion y salario. El salario tendrá in atributo con el tipo de moneda. La dirección estará formada por la calle, localidad y codigo postal. Además, todas las personas tendrán un identificador "id" como atributo.
Los datos son los siguientes:

- Persona1
  - Pedro Parra "el jefe"
  - pedro@kk.com
  - calle Huercal,4, Almeria, 70300
  - 1000€
  - id:100
- Persona2
  - Alicia Parra
  - alicia@kk.com
  - calle Huercal,4, Almeria, 70300
  - 1500€
  - id:101
- Persona3
  - Mario Perez&Santos Almeida
  - mario@kk.com
  - calle Huercal,4, Almeria, 70300
  - 2000€
  - id:102


## Ejercicio05

Crear un XML para representar el albun musical de El Madrileño, de C.Tangana.  
Se libre de indicar los campos que consideres, con la siguiente consideración:
- Hay que indicar dos generos, Pop y Folk
- No es necesario meter todas las canciones, solo las 3 primeras 
- Imagina que el albun tiene el ISBN de "111-111-111-111". Ponlo como atributo.
- ¿Se puede meter la portada del disco en un XML?

<img src="caratula.png" width="100">


## Ejercicio06 - busqueda de errores
El siguiente fragmento de código XML contiene **7 errores** sintácticos que impiden que sea un documento bien formado. Localiza los errores, indícalos brevemente y reescribe el código de forma correcta. Usa entidades para " y >.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<tienda>
  <!-- Catálogo de productos ->
  <Producto id=A01>
    <nombre>Monitor 27"</nombre>
    <precio moneda="EUR">199.99</precio>
    <descripcion>Pantalla IPS con relación de aspecto > 16:9</descripcion>
    <stock>12</producto>
  <producto id="A02">
    <nombre>Ratón Gaming</nombre>
    <precio moneda="EUR">25.00</precio>
    <stock>0</stock>
  </producto>
</tienda>
```

## Ejercicio07 - espacio de nombres
Primero, documentate sobre como usar espacios de nombres (namespaces) en XML. Para ello, puedes visitar [esta web](https://www.eniun.com/espacios-de-nombres-xml/)

Escribe un ejemplo de documento XML que utilice namespaces para evitar colisiones de nombres. El documento describirá un albun musical y un libro, de una tienda genérica. En ambos productos, tendremos _titulo_, _autor_ y _genero_. 


# Ejercicio08 - equivalencia XML/JSON

Transforma el siguiente JSON en XML

```JSON
{
  "biblioteca": {
    "libro": [
      {
        "titulo": "El señor de los anillos",
        "autor": "J.R.R. Tolkien",
        "genero": "Fantasía"
      },
      {
        "titulo": "Cien años de soledad",
        "autor": "Gabriel García Márquez",
        "genero": "Realismo mágico"
      }
    ]
  }
}
``` 