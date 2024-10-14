# Monitoreo de Sitio Web con Gráfico de Tiempos de Respuesta

Este proyecto es una aplicación Blazor que monitoriza el tiempo de respuesta de un sitio web específico, mostrando los resultados en un gráfico de línea en tiempo real. Utiliza `MudBlazor` para la visualización gráfica y `HttpClient` para verificar la disponibilidad de la página web.

## Descripción

La aplicación realiza las siguientes funciones:

- Muestra la hora de ejecución actualizada cada segundo.
- Verifica cada 4 segundos el tiempo de respuesta de un sitio web (por defecto, `https://soundcloud.com/discover`).
- Muestra un gráfico de línea con los últimos 10 tiempos de respuesta, usando `MudBlazor`.
- Si hay menos de 4 datos, muestra un mensaje indicando que está esperando más datos para dibujar el gráfico.

## Librerías

- **Blazor**: Framework para la creación de aplicaciones web interactivas con C#.
- **MudBlazor**: Biblioteca de componentes UI para Blazor que facilita la creación de interfaces gráficas modernas.
- **HttpClient**: Para realizar solicitudes HTTP y medir el tiempo de respuesta.
- **System.Timers**: Para la actualización de la hora y la verificación del tiempo de respuesta de la página.

## Requisitos

- .NET 7.
- Un navegador compatible con Blazor.
- Conexión a internet para verificar el tiempo de respuesta del sitio web.
