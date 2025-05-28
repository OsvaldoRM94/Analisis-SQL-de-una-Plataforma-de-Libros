# 📚 Análisis SQL de una Plataforma de Libros

Durante la pandemia, las dinámicas sociales cambiaron drásticamente: las personas pasaron más tiempo en casa y redescubrieron el gusto por la lectura. Este proyecto analiza una base de datos de una startup que busca posicionarse en el creciente mercado de apps para lectores. A través de consultas SQL, se exploran patrones y tendencias clave para generar una propuesta de valor que impulse su desarrollo.

---

## 🎯 Objetivos

- Explorar la base de datos relacional de una plataforma digital de libros.
- Obtener insights que sirvan para decisiones estratégicas del producto.
- Practicar consultas SQL con un enfoque analítico aplicado al mundo real.

---

## 🗃️ Estructura de la Base de Datos

La base de datos está compuesta por cinco tablas principales:

### `books`
Contiene información sobre los libros.
- `book_id` — ID del libro  
- `author_id` — ID del autor o autora  
- `title` — Título del libro  
- `num_pages` — Número de páginas  
- `publication_date` — Fecha de publicación  
- `publisher_id` — ID de la editorial  

### `authors`
Contiene información de autores.
- `author_id` — ID del autor o autora  
- `author` — Nombre del autor o autora  

### `publishers`
Contiene información de editoriales.
- `publisher_id` — ID de la editorial  
- `publisher` — Nombre de la editorial  

### `ratings`
Contiene calificaciones de usuarios.
- `rating_id` — ID de la calificación  
- `book_id` — ID del libro  
- `username` — Usuario que calificó  
- `rating` — Calificación otorgada  

### `reviews`
Contiene reseñas escritas por los usuarios.
- `review_id` — ID de la reseña  
- `book_id` — ID del libro  
- `username` — Usuario que escribió la reseña  
- `text` — Texto de la reseña  

---

## 🧩 Consultas Realizadas

1. 📅 Número de libros publicados después del 1 de enero de 2000.
2. ⭐ Número de reseñas de usuarios y calificación promedio para cada libro.
3. 🏢 Editorial con mayor número de libros con más de 50 páginas.
4. ✍️ Autor con la calificación promedio más alta (solo libros con al menos 50 calificaciones).
5. 💬 Número promedio de reseñas de texto entre usuarios que calificaron más de 50 libros.

---

## ⚙️ Tecnologías Utilizadas

- **Lenguaje:** SQL (PostgreSQL)
- **Entorno:** Jupyter Notebook
- **Librerías:**  
  - `pandas` — Para visualizar resultados  
  - `sqlalchemy` — Para establecer la conexión a la base de datos  
  - `psycopg2` — Driver de conexión PostgreSQL  

---

## 📝 Conclusiones

> A través del análisis de datos realizado, se identificaron oportunidades importantes para la estrategia del producto, como:
>
> - Editoriales clave que publican libros más extensos, ideales para usuarios intensivos.
> - Autores con alto engagement por sus calificaciones promedio.
> - Usuarios altamente activos (más de 50 calificaciones) que podrían ser embajadores o testers del producto.
> - Preferencias del público en cuanto a títulos con mayor interacción (reseñas y calificaciones).

---

## 📎 Notas

- Todas las consultas fueron realizadas exclusivamente con SQL.
- Se utilizó `pandas` únicamente para mostrar y almacenar los resultados.
- Este proyecto forma parte del bootcamp de analista de datos de [TripleTen](https://tripleten.com).

---
