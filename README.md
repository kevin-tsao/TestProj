# TestProj

This repository contains a sample .NET 8 Web API project that demonstrates JWT authentication.

## Running the API

The `JwtAuthApi` project targets .NET 8.0. You can build and run the API using the `dotnet` CLI:

```bash
dotnet restore JwtAuthApi/JwtAuthApi.csproj
dotnet run --project JwtAuthApi/JwtAuthApi.csproj
```

The API exposes two endpoints:

- `POST /Auth/login` – accepts a JSON body with `username` and `password` and returns a JWT token when the credentials are valid (default user/password is `user`/`password`).
- `GET /WeatherForecast` – a protected endpoint that requires a valid JWT Bearer token in the `Authorization` header.

Swagger UI is enabled in development to facilitate testing.
