# Utilisez une image Python officielle de Docker Hub
FROM python:3.8-slim-buster

# Définissez le répertoire de travail dans le conteneur
WORKDIR /app

# Copiez les fichiers de dépendances dans le répertoire de travail
COPY requirements.txt .

# Installez les dépendances
RUN pip install --no-cache-dir -r requirements.txt

# Copiez le code source dans le répertoire de travail
COPY . .

# Exécutez l'application
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]