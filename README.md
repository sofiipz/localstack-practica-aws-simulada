# LocalStack 

Esta práctica consiste en la simulación de algunos servicios de Amazon Web Services (AWS) utilizando **LocalStack**, una plataforma que permite emular estos servicios de forma local sin necesidad de conectarse a AWS real.

Se trabaja principalmente con los servicios:
- **S3** (almacenamiento de objetos)
- **Lambda** (funciones serverless)

La práctica se realiza sobre **Docker Desktop** utilizando **WSL (Ubuntu)** como entorno de integración.

---

## 🧪 Estructura de la práctica

### 🔹 Parte 1 - Preparación del entorno

- Instalación y configuración de Docker Desktop y WSL.
- Instalación de la extensión de LocalStack.
- Configuración del contenedor y de las credenciales con `aws configure`.

### 🔹 Parte 2 - Servicio S3

- Creación de buckets: `sofia-bucket-provisional` y `sofia-bucket-definitivo`.
- Subida de archivos y verificación desde terminal.
- Copia de archivos entre buckets.
- Descarga y lectura de archivos desde el contenedor.
- Eliminación de bucket provisional.

### 🔹 Parte 3 - Funciones Lambda

- Creación de un archivo `handler.py` con una función que recibe un parámetro.
- Comprimir en `.zip` y mover al entorno de LocalStack.
- Creación y ejecución de la función Lambda.
- Análisis del archivo `respuesta.json` con error esperado debido a limitaciones de LocalStack.

> ⚠️ Nota: El error `"Runtime.HandlerNotFound"` es el resultado esperado en LocalStack Community y **no impide que se dé por válida esta parte de la práctica**.

---

## 📅 Fecha: Abril de 2025

