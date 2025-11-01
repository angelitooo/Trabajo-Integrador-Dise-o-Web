CRUD "Tareas" — Entregable práctico (PHP + React)
=================================================

Estructura:
- /api       -> API en PHP (archivo único index.php). Almacena datos en tasks.json.
- /frontend  -> App React (Vite) con Hooks.

Cómo ejecutar :
Usando Visual Studio Code, desde un terminal ingresar a la carpeta del proyecto.
En mi caso , Agregar area de trabajo desde el editor, y luego abrir un terminal desde donde abrir la carpeta del proyecto.
Luego, seguir los siguientes pasos: 

1) Backend (PHP builtin server, puerto 8000):
   Desde la carpeta del proyecto:
     php -S 0.0.0.0:8000 -t api
   Sirve la carpeta /api como raíz. La API queda disponible en http://localhost:8000

2) Frontend (React + Vite, puerto 5173):
   cd frontend
   npm install
   npm run dev
   -> Vite por defecto usa el puerto 5173 (puede cambiar si está ocupado)

Rutas de la API (base: http://localhost:8000):
- GET  /tasks                 -> listar tareas
- POST /tasks                 -> crear tarea (JSON body: {"title":"..."})
- POST /tasks/{id}/complete   -> marcar tarea como completada
- DELETE /tasks/{id}          -> borrar tarea



