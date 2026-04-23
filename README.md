# SPIR v7.0 - Sistema de Planificación Inteligente de Redes

# Descripción
SPIR v7.0 es una plataforma web integral diseñada para la planificación, automatización y gestión de infraestructuras de red. Desarrollada como una solución de Infraestructura como Código (IaC), esta herramienta permite a los ingenieros de red simular, configurar y monitorear dispositivos de red de manera eficiente, optimizando el flujo de trabajo y reduciendo errores manuales. Su última versión incorpora un avanzado motor de Detección Real de Dispositivos que permite interactuar con hardware físico en una red local.
Este proyecto es ideal para entornos educativos y laboratorios, proporcionando una experiencia práctica en la gestión de redes modernas.

## Características principales
SPIR v7.0 se divide en dos etapas principales, ofreciendo un conjunto robusto de funcionalidades:
**Etapa 1: Planificación de Red**
* **Gestión de Edificios:** Permite definir y organizar la infraestructura de red por ubicaciones físicas, facilitando la escalabilidad y el control.
* **Planificación IP Automática:** Genera esquemas de direccionamiento IP de forma inteligente, asignando subredes y rangos DHCP para evitar conflictos y optimizar el uso del espacio de direcciones.
* **Segmentación VLAN:** Facilita la creación y gestión de VLANs, mejorando la seguridad y el rendimiento de la red mediante la segmentación del tráfico.
* **Topología Visual Interactiva:** Renderiza diagramas de red dinámicos que muestran la interconexión de dispositivos y edificios, ofreciendo una visión clara de la infraestructura.
* **Generador de Comandos Multimarca:** Produce comandos de configuración específicos para diferentes fabricantes (Cisco IOS, Huawei VRP, Fortinet FortiOS, Arista EOS), asegurando la compatibilidad y reduciendo la curva de aprendizaje.
**Etapa 2: Automatización y Operaciones**
* **Auto-Discovery Real de Dispositivos:** Una característica innovadora que permite a la plataforma escanear la red local y detectar dispositivos físicos (routers, switches, APs) conectados al PC. Utiliza peticiones HTTP/S a puertos comunes y rangos IP predefinidos para identificar equipos activos.
* **Gestión de Dispositivos Registrados:** Mantiene un inventario centralizado de los dispositivos detectados y agregados, permitiendo una administración sencilla.
* **Despliegue de Configuración:** Simula y ejecuta el despliegue de configuraciones generadas a los dispositivos de red, con opciones de Dry-Run para validación previa.
* **Monitoreo en Tiempo Real:** Proporciona una visión básica del estado operativo de los dispositivos, mostrando métricas simuladas de CPU, RAM e interfaces.
* **Auditoría Completa:** Registra todas las acciones y cambios realizados en la plataforma, garantizando la trazabilidad y facilitando la resolución de problemas.

## Arquitectura del sistema
El sistema está construido como una **Single Page Application (SPA)** en un único archivo HTML:
* **HTML:** estructura de la interfaz
* **CSS:** estilos y diseño responsivo
* **JavaScript:** lógica del sistema y simulación de operaciones

## Módulos del sistema
* **Planificación Inicial:** Utiliza los módulos de Gestión de Edificios y Planificación IP para diseñar la estructura lógica de tu red.
* **Segmentación:** Define tus VLANs en el módulo de Segmentación VLAN.
* **Visualización:** Genera la Topología para obtener una representación gráfica de tu diseño.
* **Generación de Comandos:** Crea las configuraciones específicas para tus dispositivo usando el Generador de Comandos.
* **Detección de Hardware:** Navega al módulo de Auto-Discovery y haz clic en "Detectar Dispositivos" para encontrar equipos reales en tu red.
* **Gestión y Despliegue:** Agrega los dispositivos detectados a tu inventario y utiliza los módulos de Despliegue y Monitoreo para gestionar y operar tu infraestructura.
* **Auditoría:** Revisa el Registro de Auditoría para mantener un control de todas las acciones realizadas.

## Tecnologías utilizadas
* **Frontend:** HTML5, CSS3, JavaScript (Vanilla JS)
* **Iconografía:** Font Awesome 6.4.0
* **Fuentes:** Google Fonts (Segoe UI, Tahoma, Geneva, Verdana)
* **Conceptos de Redes:** CIDR, VLANs, SSH, Telnet, HTTP/S, ICMP
* **Metodologías:** Infraestructura como Código (IaC), Fuente Única de Verdad (SoT)

## Cómo usar el sistema
Este proyecto es una aplicación web autónoma contenida en un único archivo HTML. No requiere instalación de servidores o dependencias complejas.
* **Descarga el archivo:** Sistema de Planificación Inteligente de Redes v7.html de este repositorio.
* **Abre en el Navegador:** Simplemente abre el archivo Sistema de Planificación Inteligente de Redes v7.html con tu navegador web preferido (Chrome, Firefox, Edge, etc.).
* **Conecta tus Dispositivos:** Para utilizar la función de Auto-Discovery Real, asegúrate de que tus dispositivos de red (switches, routers, etc.) estén conectados físicamente a la misma red que tu PC y que tengan direcciones IP configuradas en rangos comunes (ej.192.168.1.x , 10.0.0.x ).

## Limitaciones
* La aplicación funciona completamente en el frontend (sin backend ni base de datos)
* No se cuenta con autenticación de usuarios ni control de acceso

## Autor
Yeraldin Miranda Barbosa
Fundación Universitaria Compensar
Ingeneria en Telecomunicaciones
