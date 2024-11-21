
![BG_ZOOM_ONE_ESP_(1) 1](https://github.com/nandojmj/Alura_Challenge_Literatura/assets/156966097/df2ed853-d338-4ba8-b8f3-e53b101b1eff)

## Open Challenge Backend ONE G7- LITERATURA
 ***ONE | Fase 3 - Especialización Back-End  G7 Alura - Oracle Next Education***



Este es un desafío de la Especialización __Back-End G7 Alura - Oracle Next Education.__ El proyecto se llama "Alura Literatura" y es una aplicación que permite a los usuarios consultar información sobre libros y autores, un catálogo de libros. Está diseñado para interactuar con una base de datos PostgreSQL para almacenar información sobre libros y autores, y proporciona funcionalidades como búsqueda, listado y consulta de datos relacionados con libros y autores. A continuación, se detallan las clases principales y su funcionalidad:

Los pasos solicitados para completar este desafío:

1.  Configurando el entorno Java y Spring
2.	Conociendo la API para traer datos
3.	Construyendo una solicitud de API
- 3.1	Construyendo el Cliente para Solicitudes (HttpClient)
- 3.2	Construyendo la Solicitud (HttpRequest)
- 3.3	Construyendo la la Respuesta (HttpResponse)
4.	Analizando la respuesta en formato JSON
5.	Convertiendo los datos
6.	Interactuando con el usuario
7.	Consultando Libros
8.	Consultando Autores
9.	Persistencia de datos
10. Listando libros por idiomas
11.  Listando autores vivos en determinado año
12. Hacer un Readme.md
13. Extra (Opcional)
- 13.1 Generando estadísticas
- 13.2 Top 10 libros más descargados
- 13.3 Buscar autor por nombre
- 13.4 Listar autores con otras consultas
    
   
&nbsp;

> [!NOTE]
> En este Challenge se solicita primero crear el repositorio del proyecto en GitHub.  
> El siguiente material te ayudará con esta actividad: [Git - Configurando Git por primera vez](https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Configurando-Git-por-primera-vez) y [Como subir mi proyecto en GitHub](https://www.youtube.com/watch?v=bhKkeOMysuw)  

&nbsp;



### Clases Principales:
#### Principal (com.alura.literatura.principal.Principal):

- Esta clase parece ser la clase principal de la aplicación. Contiene el método muestraElMenu() que muestra un menú de opciones al usuario y maneja la interacción con el usuario.
- Utiliza instancias de LibroRepository y AutorRepository para acceder a la base de datos y realizar operaciones CRUD en las entidades Libro y Autor.

#### Libro (com.alura.literatura.model.Libro):

- Esta clase representa la entidad "Libro" en el modelo de datos de la aplicación.
- Tiene atributos como id, titulo, autor, idioma y descargas.
- Está mapeada a una tabla llamada "libros" en la base de datos.
- La clase proporciona métodos para acceder y modificar sus atributos, así como un método toString() para imprimir información sobre el libro.

#### Autor (com.alura.literatura.model.Autor):

- Esta clase representa la entidad "Autor" en el modelo de datos de la aplicación.
- Tiene atributos como id, nombre, fechaNacimiento y fechaFallecimiento.
- Está mapeada a una tabla llamada "autores" en la base de datos.
- La clase proporciona métodos para acceder y modificar sus atributos, así como un método toString() para imprimir información sobre el autor.

#### LibroRepository (com.alura.literatura.repository.LibroRepository):

- Esta interfaz proporciona métodos para realizar operaciones CRUD en la entidad Libro.
- Extiende JpaRepository de Spring Data JPA.

#### AutorRepository (com.alura.literatura.repository.AutorRepository):

- Esta interfaz proporciona métodos para realizar operaciones CRUD en la entidad Autor.
- Extiende JpaRepository de Spring Data JPA.

#### LiteraturaApplication (com.alura.literatura.LiteraturaApplication):

- Esta clase es la clase principal de Spring Boot que inicia la aplicación.
- Implementa CommandLineRunner y utiliza instancias de LibroRepository y AutorRepository para iniciar la aplicación y mostrar el menú principal.
  
### Servicios y Utilidades:
#### AutorServicio (com.alura.literatura.service.AutorServicio):

- Este servicio proporciona métodos para obtener información sobre autores.
- Utiliza AutorRepository para acceder a la base de datos y obtener datos sobre autores.

#### LibroServicio (com.alura.literatura.service.LibroServicio):

- Este servicio proporciona métodos para obtener información sobre libros.
- Utiliza LibroRepository para acceder a la base de datos y obtener datos sobre libros.

#### ConvierteDatos (com.alura.literatura.service.ConvierteDatos) y ConvierteDatosAutor (com.alura.literatura.service.ConvierteDatosAutor):

- Estas clases proporcionan métodos para convertir datos de JSON a objetos Java utilizando la biblioteca Jackson ObjectMapper.
- Implementan la interfaz IConvierteDatos.



```

```sql

Copyright (c) [2024] [Fredy Mamani Mamani J]

Se concede permiso, de forma gratuita, a cualquier persona que obtenga una copia
de este software y de los archivos de documentación asociados (el "Software"), para tratar
con el Software sin restricciones, incluyendo sin limitación los derechos
para usar, copiar, modificar, fusionar, publicar, distribuir, sublicenciar y/o vender
copias del Software, y para permitir a las personas a las que se les proporcione el Software
para hacerlo, sujeto a las siguientes condiciones:

El aviso de copyright anterior y este aviso de permiso se incluirán en todas las
copias o porciones sustanciales del Software.

EL SOFTWARE SE PROPORCIONA "TAL CUAL", SIN GARANTÍA DE NINGÚN TIPO, EXPRESA O
IMPLÍCITA, INCLUYENDO PERO NO LIMITADO A LAS GARANTÍAS DE COMERCIABILIDAD,
IDONEIDAD PARA UN PROPÓSITO PARTICULAR Y NO INFRACCIÓN. EN NINGÚN CASO LOS
AUTORES O TITULARES DE DERECHOS DE AUTOR SERÁN RESPONSABLES DE CUALQUIER RECLAMO, DAÑOS U OTROS
RESPONSABILIDAD, YA SEA EN UNA ACCIÓN DE CONTRATO, AGRAVIO O DE OTRO MODO, QUE SURJA DE,
FUERA O EN RELACIÓN CON EL SOFTWARE O EL USO U OTROS TRATOS EN EL
SOFTWARE.


# literatura_alura
