# 📘 Examen Práctico - Unidad II  
### ALBERT KENYI APAZA CCALLE  
**Código:** 2021071075  

---

## 🔖 Historias de Usuario Implementadas

| Código | Descripción |
|--------|-------------|
| **H04** | Permitir ver detalles de riesgo al tocar una zona del mapa. |
| **H06** | Permitir al usuario ingresar origen y destino, calcular ruta priorizando seguridad y mostrarla visualmente en el mapa. |

---

## 📱 Capturas de Funcionalidad

### 🔹 H04 - Ver detalles de riesgo al tocar una zona del mapa

| Paso | Descripción | Imagen |
|------|-------------|--------|
| 1 | Login con Firebase | ![](imagenesReadme/1Login.png) |
| 2 | Selección de marcador y visualización de riesgos | ![](imagenesReadme/2SeleccionarAlternarRutasMarcadores.png) |
| 3 | Solicitud de permiso de ubicación | ![](imagenesReadme/3H04PreguntaUbicacionActual.png) |
| 4 | Solicitud del sistema para acceder a la ubicación | ![](imagenesReadme/4H04SolicitudUbicacionActual.png) |
| 5 | Ubicación actual mostrada en el mapa | ![](imagenesReadme/5H04SitioActual.png) |


---

### 🔹 H06 - Ruta segura: origen, destino y visualización

| Paso | Descripción | Imagen |
|------|-------------|--------|
| 1 | Ingresar punto de origen | ![](imagenesReadme/6H04Origen.png) |
| 2 | Ingresar punto de destino | ![](imagenesReadme/7H04Destino.png) |
| 3 | Visualización de ambos puntos | ![](imagenesReadme/8H04OrigenDestino.png) |
| 4 | Ruta segura trazada en el mapa | ![](imagenesReadme/9H04TrazarRuta.png) |

---

## 🧰 Tecnologías y APIs Utilizadas

- **Flutter** (Desarrollo multiplataforma)
- **Firebase** (Autenticación y backend)
- **Google Maps API** (Visualización de mapas)
- **Google Maps Routes API** (Trazado de rutas seguras)
- **Google Places API** (Búsqueda y autocompletado de lugares)

---

## 📌 Diagrama de Flujo (Mermaid)


graph TD
    A[Inicio] --> B[Login con Firebase]
    B --> C[Solicitar ubicación al usuario]
    C --> D[Mostrar mapa con ubicación actual]
    D --> E[Seleccionar zona de riesgo]:::riesgo
    E --> F[Mostrar detalles del riesgo]
    D --> G[Ingresar origen y destino]:::ruta
    G --> H[Calcular ruta segura]
    H --> I[Mostrar ruta segura en el mapa]
