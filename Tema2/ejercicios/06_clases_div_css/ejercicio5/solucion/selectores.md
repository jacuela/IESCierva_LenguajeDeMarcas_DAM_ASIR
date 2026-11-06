# Lista de selectores Ejercicio5

Los dos productos (los dos div)  
`.producto`

---

Solo el producto que está de oferta.    
`.oferta`

---

Todos los elementos con la clase precio.  
`.precio`

---

Los precios de los productos, pero no el texto del envío.
Con .precio solo, también se seleccionaría el envío (línea 18).  
`.producto .precio`
---

El título del producto en oferta (y ningún otro).
h2 seleccionaría también el título del teclado.  
`.oferta h2`
---

Todos los párrafos de la cabecera.  
`.cabecera p`
---

Todos los span que hay dentro de un producto.   
`.producto span`
---

Los colores (negro y blanco), y nada más.
`span` solo seleccionaría también el precio
span antiguo.  
`.color`

---

El precio antiguo que hay dentro del precio del producto en oferta.   
`.oferta .precio .antes`