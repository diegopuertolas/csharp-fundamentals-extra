# C# Fundamentals - Ejercicios 

- [Restaurant](#restaurant)
- [Videogame](#videogame)
- [Streaming Platform](#streaming-platform)
- [Library](#library)
- [Parking](#parking)
- [Shop](#shop)
- [ATM](#atm)
- [Guess the number](#guess-the-number)
- [Gym](#gym)
- [MultimediaCatalog](#multimedia-catalog)

## Restaurant

[Ir al Repositorio](https://github.com/diegopuertolas/Restaurant)

[↓ Descargar código (.zip) (v1.0.0)](https://github.com/diegopuertolas/Restaurant/archive/refs/tags/v1.0.0.zip)

## Videogame

[Ir al Repositorio](https://github.com/diegopuertolas/Videogame)

[↓ Descargar código (.zip) (v1.0.0)](https://github.com/diegopuertolas/Videogame/archive/refs/tags/v1.0.0.zip)

<details>

<summary>Haz clic aquí para ver el enunciado</summary>

### Enunciado

Crear una clase abstracta:

```csharp
Personaje
```

con las propiedades:

- Nombre.
- Vida.

Definir el método:

```csharp
public abstract string ObtenerDescripcion();
```

Crear las siguientes clases:

```text
Personaje
 |
 +-- Guerrero
 |
 +-- Mago
 |
 +-- Arquero
```

Cada clase tendrá una propiedad específica:

- `Guerrero`: Fuerza.
- `Mago`: Mana.
- `Arquero`: NumeroFlechas.

Crear varios personajes y almacenarlos en:

```csharp
List<Personaje>
```

Recorrer la colección y mostrar la descripción de cada personaje.

Responder:

1. ¿Por qué `Personaje` puede ser una clase abstracta?
2. ¿Por qué un `Mago` puede almacenarse en una variable de tipo `Personaje`?
3. ¿Qué método `ObtenerDescripcion()` se ejecutará para cada objeto?

</details>

## Streaming Platform

[Ir al Repositorio](https://github.com/diegopuertolas/StreamingPlatform)

[↓ Descargar código (.zip) (v1.0.0)](https://github.com/diegopuertolas/StreamingPlatform/archive/refs/tags/v1.0.0.zip)

<details>

<summary>Haz clic aquí para ver el enunciado</summary>

### Enunciado

Una plataforma dispone de diferentes tipos de contenido.

Crear una clase abstracta:

```csharp
Contenido
```

con las propiedades:

- Título.
- Duración.

Crear:

```text
Contenido
 |
 +-- Pelicula
 |
 +-- Serie
 |
 +-- Documental
```

Cada clase tendrá además información específica.

##### Pelicula

- Director.

##### Serie

- Número de temporadas.

##### Documental

- Temática.

La clase `Contenido` definirá:

```csharp
public abstract string ObtenerDescripcion();
```

Cada clase hija deberá implementar el método.

Crear:

- 2 películas.
- 2 series.
- 1 documental.

Almacenar todos los objetos en:

```csharp
List<Contenido>
```

Recorrer la colección y mostrar la descripción de cada contenido.

#### Buscar contenido

Solicitar al usuario:

```text
Título a buscar:
```

Buscar el contenido recorriendo la colección.

La búsqueda no deberá depender de mayúsculas y minúsculas.

Si existe:

```text
Contenido encontrado:

Interstellar - 169 minutos
```

Si no existe:

```text
No se ha encontrado el contenido.
```

Resolver sin utilizar LINQ.

#### Filtrar películas

Utilizando la colección del ejercicio de streaming, mostrar solamente los objetos que sean de tipo `Pelicula`.

Utilizar el operador:

```csharp
is
```

Después, modificar el programa para mostrar únicamente las series.

Responder:

1. ¿De qué tipo es la colección?
2. ¿De qué tipo es la variable utilizada en el `foreach`?
3. ¿Cómo puede el programa saber si un determinado `Contenido` es realmente una `Pelicula`?

</details>

## Library

[Ir al Repositorio](https://github.com/diegopuertolas/Library)

[↓ Descargar código (.zip) (v1.0.0)](https://github.com/diegopuertolas/Library/archive/refs/tags/v1.0.0.zip)

<details>

<summary>Haz clic aquí para ver el enunciado</summary>

### Enunciado

Crear una clase abstracta:

```csharp
Publicacion
```

con:

- Título.
- Año de publicación.

Crear:

```text
Publicacion
 |
 +-- Libro
 |
 +-- Revista
 |
 +-- Comic
```

Añadir una propiedad específica a cada clase.

Por ejemplo:

- `Libro`: Autor.
- `Revista`: Número.
- `Comic`: Dibujante.

Todas las publicaciones deberán implementar:

```csharp
ObtenerDescripcion()
```

Crear diferentes objetos y almacenarlos en:

```csharp
List<Publicacion>
```

Mostrar posteriormente todas las publicaciones.

#### Publicaciones por año

Solicitar:

```text
Mostrar publicaciones posteriores al año:
```

Validar el dato mediante:

```csharp
int.TryParse()
```

Mostrar solamente las publicaciones cuyo año sea superior al indicado.

Si el usuario introduce un valor que no sea un número, mostrar un mensaje de error.

Resolver sin utilizar LINQ.

</details>

## Parking

[Ir al Repositorio](https://github.com/diegopuertolas/Parking)

[↓ Descargar código (.zip) (v1.0.0)](https://github.com/diegopuertolas/Parking/archive/refs/tags/v1.0.0.zip)

<details>

<summary>Haz clic aquí para ver el enunciado</summary>

### Enunciado

Crear una clase abstracta:

```csharp
Vehiculo
```

con:

- Matrícula.
- Marca.

Crear las clases:

```text
Vehiculo
 |
 +-- Coche
 |
 +-- Moto
 |
 +-- Furgoneta
```

Añadir al menos una propiedad específica a cada clase.

Crear varios vehículos y almacenarlos en:

```csharp
List<Vehiculo>
```

Crear un menú:

```text
=== PARKING ===

1. Ver vehículos
2. Buscar por matrícula
3. Mostrar coches
0. Salir
```

El programa deberá continuar funcionando hasta seleccionar la opción `0`.

Separar cada operación en un método.

#### Validar el menú

El programa deberá controlar entradas como:

```text
Pepe
-1
25
2.5
```

Utilizar `TryParse()`.

Una entrada incorrecta no deberá finalizar la aplicación.

</details>

## Shop

[Ir al Repositorio](https://github.com/diegopuertolas/Shop)

[↓ Descargar código (.zip) (v1.0.0)](https://github.com/diegopuertolas/Shop/archive/refs/tags/v1.0.0.zip)

<details>

<summary>Haz clic aquí para ver el enunciado</summary>

### Enunciado

#### Precio más barato

Crear una clase:

```csharp
Articulo
```

con:

- Nombre.
- Precio.

Crear varios artículos y almacenarlos en:

```csharp
List<Articulo>
```

Recorrer la colección y localizar el artículo con el precio más bajo.

Ejemplo:

```text
El artículo más barato es:

Cable USB - 4,50 €
```

#### Precio medio

Calcular el precio medio de todos los artículos.

El resultado deberá calcularse a partir de los objetos almacenados en la colección.

No se indicará manualmente el número de artículos.

Ejemplo:

```text
Precio medio: 23,45 €
```

#### Buscar por precio máximo

Solicitar:

```text
Precio máximo:
```

Validar el valor utilizando:

```csharp
decimal.TryParse()
```

Mostrar todos los artículos cuyo precio sea igual o inferior al indicado.

Si no existe ninguno, mostrar un mensaje.

</details>


## ATM

[Ir al Repositorio](https://github.com/diegopuertolas/ATM)

[↓ Descargar código (.zip) (v1.0.0)](https://github.com/diegopuertolas/ATM/archive/refs/tags/v1.0.0.zip)

<details>

<summary>Haz clic aquí para ver el enunciado</summary>

### Enunciado

Crear una aplicación de consola que simule algunas operaciones básicas de un cajero.

El programa comenzará con un saldo inicial, por ejemplo:

```csharp
decimal saldo = 1000;
```

Mostrar un menú:

```text
=== CAJERO ===

1. Consultar saldo
2. Ingresar dinero
3. Retirar dinero
0. Salir
```

Requisitos:

- El menú deberá repetirse hasta seleccionar `0`.
- Utilizar `switch`.
- Validar las cantidades mediante `decimal.TryParse()`.
- No permitir ingresos negativos.
- No permitir retiradas negativas.
- No permitir retirar una cantidad superior al saldo.
- Separar las operaciones en métodos.

No es necesario utilizar clases para este ejercicio.

</details>

## Guess The Number

[Ir al Repositorio](https://github.com/diegopuertolas/GuessTheNumber)

[↓ Descargar código (.zip) (v1.0.0)](https://github.com/diegopuertolas/GuessTheNumber/archive/refs/tags/v1.0.0.zip)

<details>

<summary>Haz clic aquí para ver el enunciado</summary>

### Enunciado

Crear un programa que genere un número aleatorio entre 1 y 100.

El usuario deberá intentar adivinarlo.

Después de cada intento, el programa indicará:

```text
El número es mayor.
```

o:

```text
El número es menor.
```

Cuando el usuario acierte:

```text
Correcto. Has necesitado 7 intentos.
```

Validar mediante `TryParse()` que el usuario introduce un número.

El programa no deberá finalizar si se introduce texto.

</details>

## Gym

[Ir al Repositorio](https://github.com/diegopuertolas/Gym)

[↓ Descargar código (.zip) (v1.0.0)](https://github.com/diegopuertolas/Gym/archive/refs/tags/v1.0.0.zip)

<details>

<summary>Haz clic aquí para ver el enunciado</summary>

### Enunciado

Desarrollar una pequeña aplicación para gestionar las actividades de un gimnasio.

Crear una clase abstracta:

```csharp
Actividad
```

Todas las actividades tendrán:

- Nombre.
- Duración.
- Número máximo de participantes.

Crear al menos:

```text
Actividad
 |
 +-- Spinning
 |
 +-- Yoga
 |
 +-- CrossTraining
```

Cada clase deberá tener alguna propiedad específica.

Definir en `Actividad` al menos un método abstracto que deba ser implementado por las clases hijas.

Crear varias actividades y almacenarlas en:

```csharp
List<Actividad>
```

La aplicación tendrá un menú similar a:

```text
=== GIMNASIO ===

1. Ver actividades
2. Buscar actividad
3. Ver actividades por duración máxima
4. Ver actividades por tipo
0. Salir
```

Requisitos:

- Utilizar herencia.
- Utilizar una clase abstracta.
- Utilizar `override`.
- Utilizar polimorfismo.
- Utilizar `List<Actividad>`.
- Utilizar `is` en alguna operación.
- Utilizar métodos.
- Pasar las colecciones mediante parámetros.
- Utilizar `while` y `switch`.
- Utilizar `TryParse()` cuando sea necesario.
- Controlar las entradas incorrectas.

No utilizar LINQ.

</details>

## Multimedia Catalog

[Ir al Repositorio](https://github.com/diegopuertolas/MultimediaCatalog)

[↓ Descargar código (.zip) (v1.0.0)](https://github.com/diegopuertolas/MultimediaCatalog/archive/refs/tags/v1.0.0.zip)

<details>

<summary>Haz clic aquí para ver el enunciado</summary>

### Enunciado

El objetivo de este ejercicio es construir una aplicación de consola en C# para administrar un catálogo de películas y series.

#### Requisitos del Sistema

##### 1. Interfaces
Crea una interfaz llamada `IEvaluable` que obligue a implementar:
* Un método `void AsignarPuntuacion(double nota)`.
* Una propiedad de solo lectura `double PuntuacionMedia { get; }`.

##### 2. Clase Abstracta Base
Crea una clase abstracta `ContenidoMultimedia` que implemente `IEvaluable`.
* **Propiedades:** `Id` (Guid o string), `Titulo` (string), `FechaEstreno` (DateTime), y una lista interna (protegida o privada) de puntuaciones (`List<double>`).
* **Implementación de Interfaz:** Lógica para añadir una nota a la lista y calcular la media. Si no hay notas, la media debe ser 0.
* **Método Abstracto:** `public abstract void MostrarDetalles();`

##### 3. Clases Derivadas (Herencia y Polimorfismo)
Crea dos clases que hereden de `ContenidoMultimedia`:

* **`Pelicula`:**
  * Propiedades extra: `Director` (string) y `DuracionMinutos` (int).
  * Sobrescribe `MostrarDetalles()` para imprimir la información específica de la película (incluyendo el director, la duración y la puntuación media).

* **`Serie`:**
  * Propiedades extra: `NumeroTemporadas` (int) y `EnEmision` (bool).
  * Sobrescribe `MostrarDetalles()` para imprimir la información adaptada a las series.

##### 4. Utilidades (Utils y Fechas)
Crea una clase estática `DateUtils`.
* **Método `FormatearFechaPublicacion(DateTime fecha)`:** Debe devolver un string con un formato amigable. Por ejemplo: *"Estrenado el 15 de Octubre de 2023"*.
* **Método `ParsearFecha(string fechaTexto)`:** Debe intentar convertir (con `TryParse` o `TryParseExact`) un string introducido por el usuario en consola a un objeto `DateTime`. Si falla, debe devolver una fecha por defecto o solicitarla de nuevo de forma controlada.

##### 5. Persistencia (Archivos y JSON)
Crea una clase `GestorDatos`.
* **`GuardarCatalogo(List<ContenidoMultimedia> catalogo, string ruta)`:** Serializa la lista a un archivo JSON. *(Pista: Al serializar una lista de una clase abstracta, revisa cómo configurar el serializador o usar atributos como `[JsonDerivedType]` para conservar el tipo derivado).*
* **`CartgarCatalogo(string ruta)`:** Deserializa el archivo JSON y devuelve la lista recuperada. Si el archivo no existe, debe manejar la excepción y devolver una lista vacía.

##### 6. Interfaz de Consola (Menú Principal)
Implementa un menú interactivo en tu `Program.cs` mediante un bucle `do-while` y un `switch` con las siguientes opciones:

1. **Añadir Película:** Pide los datos por consola, instancia una `Pelicula` y la añade a la lista.
2. **Añadir Serie:** Igual, pero pidiendo los datos específicos de `Serie`.
3. **Mostrar Catálogo:** Recorre la lista invocando el método polimórfico `MostrarDetalles()`. Utiliza `DateUtils` aquí para mostrar las fechas formateadas.
4. **Buscar por Título:** Pide un término de búsqueda y muestra los contenidos cuyo título contenga esa cadena (ignorando mayúsculas y minúsculas).
5. **Valorar un Contenido:** Pide el título exacto, busca el objeto en la lista y llama a `AsignarPuntuacion(...)`.
6. **Guardar Datos:** Llama a `GestorDatos` para escribir el archivo (por ejemplo, `catalogo.json`).
7. **Cargar Datos:** Llama a `GestorDatos` para sobreescribir la lista en memoria con lo que haya en el archivo JSON.
0. **Salir.**

</details>

---

*Desarrollo Web en Entorno Servidor, 2ºDAW*