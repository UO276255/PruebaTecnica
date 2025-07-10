# PruebaTecnica

Este repositorio contiene un ejemplo de proyecto Spring Boot que expone una API REST sencilla.

Para iniciar el proyecto ejecute:

```bash
cd spring-rest-demo
./gradlew bootRun
```

El endpoint `/api/auth/login` acepta un `email` y `password` y devuelve un token JWT que se debe incluir en la cabecera `Authorization` como `Bearer <token>` para acceder al resto de la API.

Los tokens caducan tras una hora. Para obtener uno nuevo puede llamarse a `/api/auth/refresh` enviando el token actual en la cabecera `Authorization`.
