# Entorno-IA

Este repositorio contiene un entorno configurado con servicios de IA utilizando Docker Compose.

## Servicios incluidos

- **Open WebUI**: Interfaz web para interactuar con modelos de IA.
- **Ollama**: Servicio para ejecutar modelos de lenguaje localmente.
- **MCPO**: Proxy seguro de MCP a OpenAPI.

## Requisitos previos

- Docker y Docker Compose instalados en su sistema
- Git para clonar el repositorio

## Despliegue con Docker Compose

1. Clone el repositorio:
   ```bash
   git clone https://github.com/tu-usuario/Entorno-IA.git
   cd Entorno-IA
   ```

2. Inicie todos los servicios:
   ```bash
   docker-compose up -d
   ```

3. Acceda a los servicios:
   - Open WebUI: [http://localhost:3000](http://localhost:3000)
   - Ollama API: [http://localhost:11434](http://localhost:11434)
   - MCPO: [http://localhost:8000](http://localhost:8000)

4. Para detener los servicios:
   ```bash
   docker-compose down
   ```

## Ejecutar MCPO por separado

Si desea ejecutar MCPO fuera de Docker Compose, consulte el [README de MCPO](./mcpo/README.md) para obtener instrucciones detalladas sobre la instalación y configuración.

## Estructura del proyecto

```
Entorno-IA/
├── docker-compose.yaml   # Configuración de Docker Compose
├── mcpo/                 # Servicio MCPO (MCP-to-OpenAPI proxy)
├── README.md             # Este archivo
```

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abra un issue o pull request para sugerencias o mejoras.

## Licencia

Consulte los archivos de licencia individuales en cada subdirectorio del proyecto. 