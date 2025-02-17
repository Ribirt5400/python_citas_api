# Proyecto API con Flask y MongoDB

Este proyecto es una API desarrollada en Flask que utiliza MongoDB como base de datos.

## Instalación y Configuración

### 1. Crear y Activar un Entorno Virtual (venv)

Antes de instalar las dependencias, es recomendable crear un entorno virtual para el proyecto:

```bash
# En Windows
python -m venv venv
venv\Scripts\activate

# En macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 2. Instalar Dependencias

Una vez activado el entorno virtual, instala las dependencias del proyecto desde `requirements.txt`:

```bash
pip install -r requirements.txt
```

### 3. Configurar Variables de Entorno

Para ejecutar Flask correctamente, define las siguientes variables de entorno:

```bash
# En Windows (cmd)
set FLASK_APP=application.py
set FLASK_ENV=development

# En macOS/Linux
export FLASK_APP=application.py
export FLASK_ENV=development
```

### 4. Ejecutar el Servidor Flask

Ejecuta el siguiente comando para iniciar el servidor y que sea accesible en la red local:

```bash
flask run --host=0.0.0.0 --port=5000
```

El servidor se ejecutará en `http://0.0.0.0:5000/` y será accesible en la red local.

---

## Configuración de la Base de Datos MongoDB

Para que la API funcione correctamente, debes hacer una llamada a la url de la api /migracion para que se agregen los cambos a la base de datos

---

## Notas Adicionales

- Asegúrate de que MongoDB esté corriendo antes de iniciar la API.
- Para probar la API, puedes usar herramientas como Postman o `curl`.
- La documentación de la API está disponible en `/apidocs` mediante Swagger.

---
