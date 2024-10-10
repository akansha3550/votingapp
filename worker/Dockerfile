FROM mcr.microsoft.com/dotnet/sdk:5.0 AS build
WORKDIR /source

# Copy and restore dependencies
COPY . .
RUN dotnet restore

# Build the application
RUN dotnet publish -c Release -o /app

# Use a lightweight runtime image for final stage
FROM mcr.microsoft.com/dotnet/aspnet:5.0 AS runtime
WORKDIR /app
COPY --from=build /app .

# Expose the necessary port
EXPOSE 80
ENTRYPOINT ["dotnet", "worker.dll"]

