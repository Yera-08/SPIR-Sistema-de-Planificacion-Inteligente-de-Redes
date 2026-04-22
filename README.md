# SPIR v7.0 - Sistema de Planificación Inteligente de Redes

# Descripción

SPIR (Sistema de Planificación Inteligente de Redes) es una aplicación web diseñada para la gestión, planificación y automatización de infraestructuras de red.

Permite a los ingenieros de red planificar, desplegar, monitorear y auditar configuraciones, todo desde una interfaz interactiva y centralizada.

## Objetivo
Desarrollar una herramienta que facilite la planificación de redes y la automatización de tareas, integrando múltiples funcionalidades en una sola plataforma accesible desde el navegador.

## Características principales

* Planificación de redes por edificios
* Generación automática de subredes
* Configuración de VLANs
* Visualización de topologías
* Simulación de conexión a dispositivos
* Despliegue de configuraciones
* Monitoreo de dispositivos
* Auditoría de eventos
* Rollback de configuraciones
* Exportación de reportes (PDF, JSON, CSV)

## Arquitectura del sistema

El sistema está construido como una **Single Page Application (SPA)** en un único archivo HTML:

* **HTML:** estructura de la interfaz
* **CSS:** estilos y diseño responsivo
* **JavaScript:** lógica del sistema y simulación de operaciones

## Módulos del sistema

* **Planificación:** gestión de edificios y subredes
* **VLAN:** generación de configuraciones
* **Topología:** visualización de red
* **Comandos:** generación de scripts para dispositivos
* **Dispositivos:** conexión simulada (SSH/Telnet)
* **Despliegue:** ejecución de configuraciones
* **Monitoreo:** métricas en tiempo real (simuladas)
* **Auditoría:** registro de eventos
* **Rollback:** reversión de cambios
* **Reportes:** exportación de datos
* **Configuración:** ajustes del sistema



## Tecnologías utilizadas

* HTML5
* CSS3
* JavaScript (Vanilla)



## Cómo usar el sistema

1. Descargar el proyecto
2. Abrir el archivo `.html` en un navegador web
3. Navegar entre los módulos desde el menú lateral
4. Simular configuraciones y monitoreo de red



## Limitaciones

* La aplicación funciona completamente en el frontend (sin backend ni base de datos)
* No se cuenta con autenticación de usuarios ni control de acceso



## Estructura del proyecto

&#x20;index.html



## Estado del proyecto

Proyecto académico / demostrativo



## Autor

Yeraldin Miranda Barbosa



## Licencia

Este proyecto es de uso académico.

