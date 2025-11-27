# Gestor de Notas con MongoDB

## Capturas de Pantalla

### Vista Principal
<img width="1476" height="889" alt="image" src="https://github.com/user-attachments/assets/4a5ec34e-87e9-4e73-b05f-8e8b489bb1b0" />

### Crear/Editar Nota
<img width="1481" height="859" alt="image" src="https://github.com/user-attachments/assets/6e29258d-f00c-4508-98ef-44405a471fb7" />
<img width="1479" height="848" alt="image" src="https://github.com/user-attachments/assets/6acc491d-631c-40cf-8cfd-77e475f09252" />
<img width="1479" height="853" alt="image" src="https://github.com/user-attachments/assets/6bfe2bd1-8259-4b3d-bb93-86c40776fac1" />
<img width="1479" height="852" alt="image" src="https://github.com/user-attachments/assets/40c79d13-64f1-4ac8-9a8c-43f6f9209495" />

### MongoDB
<img width="1645" height="779" alt="image" src="https://github.com/user-attachments/assets/8f5e3c0f-ddd7-438e-b79a-bf669939f56a" />

## Instalación

### 1️- Clonar el Repositorio


### 2- Configurar MongoDB

- Entra a la pagina: https://cloud.mongodb.com/ y crea una cuenta gratis.
- Crea un nuevo cluster:
- Selecciona el tipo gratis que se llama M0
- Dale a crear
- Crea un usuario para la base de datos:
- Ve a donde dice "Database Access"
- Pulsa en "Add New Database User"
- Guarda bien el usuario y contraseña que pongas
- Para conectar con C#:
- Ve a "Database"
- Luego a "Clusters"
- Ahi veras tu base de datos
- Consigue tu cadena de conexion:
- Pulsa el boton "Connect"
- Elige "MongoDB for VS Code"
- Copia el texto que te aparece
- Cambia la parte donde dice tu usuario y tu contraseña por los que creaste
- Este texto lo vas a usar en el siguiente paso

### 3️- Configurar la Aplicación

#### Crear Archivo de JSON en ejectuble

1. Abre la carpeta en donde aparecen los paquetes de nuget y el .exe del form
2. Agrega ahí un archivo nombrado como "appsettings.json" 
3. Escribe en el archivo el json que esta a continuación pero reemplazando la ConnectionString por la tuya 

**Para MongoDB:**
```json
{
 "MongoDB": {
  "ConnectionString": "mongodb+srv://tuusuario:tupassword@cluster0.xxxxx.mongodb.net/",
  "DatabaseName": "GestorNotas",
  "CollectionName": "Notas"
  }
}
```

> Reemplaza `tuusuario`, `tupassword` y `cluster0.xxxxx` con tus credenciales reales de MongoDB Atlas
