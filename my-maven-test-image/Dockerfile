# Використовуємо базовий образ Java
FROM openjdk:8-jre

# Копіюємо скомпільований .jar файл у контейнер
COPY /target/simple-http-server-1.0-SNAPSHOT.jar /opt/app.jar

#COPY /root/.m2/repository/com/example/my-maven-docker-project/1.0-SNAPSHOT/my-maven-docker-project-1.0-SNAPSHOT.jar /app.jar


# Встановлюємо змінну середовища для порту 3000
ENV PORT=3000

# Вказуємо, що контейнер слухатиме на порту 3000
EXPOSE 3000

# Виконуємо нашу програму при запуску контейнера
CMD ["java", "-jar", "/opt/app.jar"]

# Запускаємо безкінечний процес, який тримає контейнер активним
#CMD ["tail", "-f", "/dev/null"]
