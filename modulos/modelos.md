# posibles modelos, acá dejo una base: 

## Modelo de datos para el módulo "Sitial de Honor".

Personaje:
    • Nombre: (texto) Nombre del personaje destacado.
    • Cargo:(texto) Relación con la universidad 
    • Descripción: (texto) Información detallada sobre el personaje.
    • Imagen: (archivo) Imagen del personaje destacado.

## Modelo de datos para el módulo "Historia de la UPR":

Evento:
    • Título: (cadena de texto) Título del evento histórico.
    • Descripción: (texto) Descripción detallada del evento.
    • Fecha: (fecha) Fecha en que ocurrió el evento.
    • Personajes presentes: (objectId[]) Arreglo de mongoid de personajes

## Modelo de datos para el módulo "Correo":

    • Se consume el de la universidad, se conecta a la base dado o a la API

## Modelo de datos para el módulo "Perfil":

Usuario:
    • Nombre: (cadena de texto) Nombre del usuario.
    • Tipo de cuenta: (cadena de texto) Estudiante — Profesor(A debatir)
    • Usuario: (cadena de texto) Información de acceso (Usar el mismo de la cuenta del intranet).
    • contraseña: (cadena de texto) Información de acceso (Usar la misma de la cuenta del intranet o pueden ser distintas, se le puede dar la opción de vincular o que sea independiente).
    • Imagen: (archivo) Foto para el perfil de usuario
    • Carrera: (cadena de texto) Carrera del estudiante(en caso de ser estudiante).
    • Email: (cadena de texto) Dirección de correo electrónico la upr (la que anteriormente escribí de conectar a los correos de upr).
    • cargo: (cadena de texto) “ejemplos si es dirigente de la FEU o algo mas se le pone el cargo”
    • Actividades: (texto) Lista de actividades realizadas si tiene un cargo(responsabilidades).

## Modelo de datos para el módulo "Noticias":

Noticia:
    • Título: (cadena de texto) Título de la noticia.
    • Contenido: (texto) Contenido de la noticia.
    • Fecha de publicación: (fecha) Fecha en que se publicó la noticia.
    • Imagen: (archivo) Imagen relacionada con la noticia.
    • Usuarios presentes: (objectId[]) Arreglo de mongoid de usuarios o personajes
