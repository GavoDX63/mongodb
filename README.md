# Gestor de Notas con MongoDB

## Capturas de Pantalla

### Vista Principal
<img width="1478" height="884" alt="image" src="https://github.com/user-attachments/assets/9275b757-3a36-4595-8abb-cc7d4a43aa27" />

### Crear/Editar Nota
<img width="1475" height="886" alt="image" src="https://github.com/user-attachments/assets/3309d0d3-d805-4a40-9d64-d4bc45bf4a27" />
<img width="1474" height="885" alt="image" src="https://github.com/user-attachments/assets/3d4e0fb1-7014-4826-905a-9b30be3c85e9" />
<img width="1478" height="882" alt="image" src="https://github.com/user-attachments/assets/9ed48551-71b5-4fe2-be0b-8f43556ed2e5" />
<img width="1474" height="883" alt="image" src="https://github.com/user-attachments/assets/0c0af6ab-a045-428a-a1ae-ab9848c6edaa" />

### MongoDB
<img width="1646" height="659" alt="image" src="https://github.com/user-attachments/assets/47443b69-40be-4773-aa77-957fbc155631" />

## Instalación

### 1️- Clonar el Repositorio

```bash
git clone https://github.com/23300764/MONGO-DB.git
cd GestorNotas_MongoDB
```

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
