# Utilise Java 17 comme environnement de base
FROM eclipse-temurin:17-jre-alpine

# Crée un dossier de travail dans l'image
WORKDIR /app

# Copie le fichier .jar généré par Maven dans l'image Docker
COPY target/*.jar app.jar

# Expose le port de ton backend (généralement 8080 ou 8089 pour Spring Boot)
EXPOSE 8089

# Commande pour démarrer l'application
ENTRYPOINT ["java", "-jar", "app.jar"]