FROM mcr.microsoft.com/dotnet/core/sdk:3.1 AS build-env
WORKDIR /app

# Copy everything else and builds
COPY . .
ENV ASPNETCORE_URLS http://*80
EXPOSE 80

ENTRYPOINT ["dotnet", "docker-app.dll"]