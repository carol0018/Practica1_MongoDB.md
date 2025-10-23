# Práctica 1: Gestión de un Catálogo de Productos con MongoDB

## Parte 1: Diseño del modelo de datos

En MongoShell escribimos "db" para saber qué base de datos está usando, nos devuelve "test". Cambiamos la base de datos a "practica1".

![alt text](<imagenes/Captura de pantalla 2025-10-21 104354.jpg>)

Insertamos el documento JSON dado en nuestra colección.

![alt text](<imagenes/Captura de pantalla 2025-10-21 104920.jpg>)

A partir del modelo JSON dado, le pedimos a ChatGPT dos documentos con distinta información pero misma estructura.

![alt text](<imagenes/Captura de pantalla 2025-10-21 110344.jpg>)
![alt text](<imagenes/Captura de pantalla 2025-10-21 110946.jpg>)
![alt text](<imagenes/Captura de pantalla 2025-10-21 111040.jpg>)

## Parte 2: Consultas sobre el catálogo

### Ejercicio 1: Encontrar portátiles de una marca con más de 8GB de RAM

![alt text](<imagenes/Captura de pantalla 2025-10-21 112240.jpg>)

### Ejercicio 2: Buscar productos con la etiqueta “oferta”

![alt text](<imagenes/Captura de pantalla 2025-10-21 112505.jpg>)

### Ejercicio 3: Incrementar el stock de un producto en 10 unidades

![alt text](<imagenes/Captura de pantalla 2025-10-21 112634.jpg>)

### Ejercicio 4: Añadir una nueva reseña (review) a un producto

![alt text](<imagenes/Captura de pantalla 2025-10-21 112857.jpg>)

## Parte 3: Agregaciones

### Construye el pipeline de agregación utilizando las etapas $unwind, $group y $sort para calcular la puntuación media de las reseñas para cada producto y ordenarlos de mayor a menor puntuación promedio. Recuerda que $unwind se usa para descomponer arreglos, $group para agrupar y calcular agregaciones como $avg, y $sort para ordenar los resultados.

![alt text](<imagenes/Captura de pantalla 2025-10-23 123205.jpg>)

## Parte 4: Ejercicios adicionales

### 1. Mostrar productos con bajo stock. Se desea mostrar todos los productos con menos de 5 unidades disponibles.

![alt text](<imagenes/Captura de pantalla 2025-10-23 123730.jpg>)

No devuelve ningún resultado porque no hay ningún producto con menos de 5 unidades.

### 2. Proyección de campos específicos. Se desea mostrar únicamente el nombre y el precio de todos los productos.

![alt text](<imagenes/Captura de pantalla 2025-10-23 124125.jpg>)

### 3. Eliminar un producto por su identificador Se desea borrar un documento concreto de la colección, por ejemplo, el producto con _id: “SKU-001”.

![alt text](<imagenes/Captura de pantalla 2025-10-23 124328.jpg>)