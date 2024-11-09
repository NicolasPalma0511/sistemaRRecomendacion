# Usa una imagen base de Python
FROM python:3.8

# Configura el directorio de trabajo
WORKDIR /app

# Copia los archivos necesarios
COPY . /app

# Instala las dependencias
RUN pip install -r requirements.txt

# Expone el puerto 5000
EXPOSE 5000

# Ejecuta la aplicación Flask
CMD ["python", "recommender.py"]
