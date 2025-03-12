# Use the .NET SDK image for development
FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build
WORKDIR /app

# Copy the project files
COPY . . 

# Install dependencies
RUN dotnet restore

# Expose the backend port
EXPOSE 5000

# Start the app in watch mode for hot reload
CMD ["dotnet", "watch", "run", "--no-launch-profile", "--urls", "http://0.0.0.0:5000"]
