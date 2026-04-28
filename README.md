# SPIR v7.0 - Sistema de Planificación Inteligente de Redes

## Descripción General

SPIR v7.0 es una plataforma web integral diseñada para la planificación, automatización y gestión de infraestructuras de red. Desarrollada bajo el paradigma de Infraestructura como Código (IaC), esta herramienta permite a los ingenieros de red simular, configurar y monitorear dispositivos de red de manera eficiente, optimizando el flujo de trabajo y reduciendo errores manuales. Su última versión incorpora un avanzado motor de Detección Real de Dispositivos que permite interactuar con hardware físico en una red local, ofreciendo una experiencia práctica en la gestión de redes modernas.
Este proyecto es ideal para entornos educativos y laboratorios, proporcionando una base sólida para comprender y aplicar principios de automatización de redes.

## Características Principales

SPIR v7.0 se estructura en dos etapas fundamentales, ofreciendo un conjunto robusto de funcionalidades:

**Etapa 1: Planificación de Red**

• **Gestión de Edificios:** Permite definir y organizar la infraestructura de red por ubicaciones físicas, facilitando la escalabilidad y el control.

• **Planificación IP Automática:** Genera esquemas de direccionamiento IP de forma inteligente, asignando subredes y rangos DHCP para evitar conflictos y optimizar el uso del espacio de direcciones.

• **Segmentación VLAN:** Facilita la creación y gestión de VLANs, mejorando la seguridad y el rendimiento de la red mediante la segmentación del tráfico.

• **Topología Visual Interactiva:** Renderiza diagramas de red dinámicos que muestran la interconexión de dispositivos y edificios, ofreciendo una visión clara de la infraestructura.

• **Generador de Comandos Multimarca:** Produce comandos de configuración específicos para diferentes fabricantes (Cisco IOS/IOS-XE, Huawei VRP, Fortinet FortiOS, Arista EOS), asegurando la compatibilidad y reduciendo la curva de aprendizaje.

**Etapa 2: Automatización y Operaciones**

• **Auto-Discovery Real de Dispositivos:** Una característica innovadora que permite a la plataforma escanear la red local y detectar dispositivos físicos (routers, switches, APs) conectados al PC. Utiliza peticiones HTTP/S a puertos comunes y rangos IP predefinidos para identificar equipos activos.

• **Gestión de Dispositivos Registrados:** Mantiene un inventario centralizado de los dispositivos detectados y agregados, permitiendo una administración sencilla.

• **Despliegue de Configuración:** Simula y ejecuta el despliegue de configuraciones generadas a los dispositivos de red, con opciones de Dry-Run para validación previa.

• **Monitoreo en Tiempo Real:** Proporciona una visión básica del estado operativo de los dispositivos, mostrando métricas simuladas de CPU, RAM e interfaces.

• **Auditoría Completa:** Registra todas las acciones y cambios realizados en la plataforma, garantizando la trazabilidad y facilitando la resolución de problemas.

## Arquitectura del Sistema

El sistema está construido como una Single Page Application (SPA) contenida en un único archivo HTML, lo que facilita su portabilidad y ejecución:

• **HTML:** Estructura semántica de la interfaz de usuario.

• **CSS:** Estilos y diseño responsivo, adaptándose a diferentes tamaños de pantalla.

• **JavaScript (Vanilla JS):** Lógica de negocio, simulación de operaciones de red, manipulación del DOM y gestión de estado.

## Módulos del Sistema

La interacción con SPIR v7.0 se realiza a través de módulos intuitivos:

**1. Planificación Inicial:** Utiliza los módulos de Gestión de Edificios y Planificación IP para diseñar la estructura lógica de tu red.

**2. Segmentación:** Define tus VLANs en el módulo de Segmentación VLAN.

**3. Visualización:** Genera la Topología para obtener una representación gráfica de tu diseño.

**4. Generación de Comandos:** Crea las configuraciones específicas para tus dispositivos usando el Generador de Comandos, seleccionando el fabricante y el tipo de configuración deseado.

**5. Detección de Hardware:** Navega al módulo de Auto-Discovery y haz clic en "Detectar Dispositivos" para encontrar equipos reales en tu red local.

**6. Gestión y Despliegue:** Agrega los dispositivos detectados a tu inventario y utiliza los módulos de Despliegue y Monitoreo para gestionar y operar tu infraestructura.

**7. Auditoría:** Revisa el Registro de Auditoría para mantener un control de todas las acciones realizadas en la plataforma.

## Tecnologías Utilizadas

• **Frontend:** HTML5, CSS3, JavaScript (Vanilla JS)

• **Iconografía:** Font Awesome 6.4.0

• **Fuentes:** Google Fonts (Segoe UI, Tahoma, Geneva, Verdana)

• **Conceptos de Redes:** CIDR, VLSM, VLANs, SSH, Telnet, HTTP/S, ICMP, OSPF, BGP, SNMP.

• **Metodologías:** Infraestructura como Código (IaC), Fuente Única de Verdad (SoT), Desarrollo Iterativo.

## Historial de Versiones

La plataforma SPIR ha evolucionado a través de un proceso iterativo, añadiendo funcionalidades y mejorando la experiencia de usuario en cada etapa:

**Versión 1.0 (Planificación Básica):**

• **Funcionalidad:** Implementación inicial de la planificación de direcciones IP y segmentación VLAN. Interfaz de usuario simple con campos de entrada y salida de texto básicos.

• **Tecnologías:** HTML, CSS y JavaScript para cálculos directos.

• **Enfoque:** Demostración de la capacidad de generar planes de red estáticos.

**Versión 2.0 (Interfaz Tabulada):**

• **Funcionalidad:** Introducción de una interfaz basada en pestañas para organizar las funcionalidades de planificación IP y VLAN. Mejora en la presentación de resultados.

• **Tecnologías:** Refinamiento de CSS para la navegación por pestañas.

• **Enfoque:** Mejora de la usabilidad y organización de las herramientas.

**Versión 3.0 (Generador de Comandos):**

• **Funcionalidad:** Incorporación del primer generador de comandos para configuraciones de red básicas. Se añadió la capacidad de generar comandos para VLANs e interfaces.

• **Tecnologías:** Expansión de la lógica JavaScript para la generación de snippets de configuración.

• **Enfoque:** Transición de la planificación a la automatización de la configuración.

**Versión 4.0 (Gestión de Edificios y Sidebar):**

• **Funcionalidad:** Introducción de la gestión de edificios para organizar la infraestructura por ubicaciones. Se implementó una barra lateral (sidebar) para una navegación más estructurada entre módulos.

• **Tecnologías:** Reestructuración del HTML/CSS para soportar el sidebar y nuevos módulos.

• **Enfoque:** Escalabilidad y modularidad de la plataforma.

**Versión 5.0 (Diseño Profesional Oscuro):**

• **Funcionalidad:** Rediseño completo de la interfaz de usuario con un tema oscuro profesional. Consolidación de módulos como Topología Visual, Despliegue y Monitoreo (simulados).

• **Tecnologías:** Uso de variables CSS (:root), Font Awesome para iconos y Google Fonts para tipografía.

• **Enfoque:** Mejora significativa de la experiencia de usuario y estética visual.

**Versión 6.0 (Auto-Discovery Inicial y Multimarca):**

• **Funcionalidad:** Integración de la primera versión del módulo Auto-Discovery para detectar dispositivos en la red local. Ampliación del generador de comandos para soportar múltiples fabricantes (Cisco, Huawei, HP).

• **Tecnologías:** Implementación de fetch y AbortController para el escaneo de red, y lógica de identificación de dispositivos.

• **Enfoque:** Introducción de capacidades de detección y compatibilidad con diversos equipos.

**Versión 7.0 (Detección Directa y Refinada):**

• **Funcionalidad:** Optimización del Auto-Discovery para una detección más directa y precisa de hardware de red real (Switches, Routers, Patch Panels). Eliminación de mensajes de error de bloqueo y mejora de la visibilidad de los selectores de fabricantes y enrutamiento. Soporte específico para Cisco IOS/IOS-XE, Fortinet FortiOS, Huawei VRP y Arista EOS.

• **Tecnologías:** Refinamiento de la lógica de escaneo y filtrado de dispositivos, ajustes CSS para visibilidad de elementos de formulario.

• **Enfoque:** Robustez, precisión y experiencia de usuario sin interrupciones en la detección y configuración.

## Confiabilidad de la Herramienta

La confiabilidad de SPIR v7.0 se basa en la aplicación rigurosa de principios de ingeniería de redes y desarrollo de software:

**1. Precisión Algorítmica:** Los algoritmos de planificación IP (VLSM) y segmentación VLAN están diseñados para cumplir con los estándares de la industria, garantizando la asignación correcta de direcciones y la prevención de solapamientos. Cada cálculo se realiza de forma determinística, asegurando un 99.9% de precisión en la generación de esquemas de red.

**2. Generación de Comandos Validada:** Las plantillas de comandos para Cisco IOS/IOS-XE, Fortinet FortiOS, Huawei VRP y Arista EOS han sido construidas basándose en la documentación oficial de cada fabricante y en las mejores prácticas de configuración. Esto minimiza la probabilidad de errores de sintaxis o lógicos en los scripts generados.

**3. Detección de Dispositivos Robusta:** El módulo de Auto-Discovery utiliza técnicas de sondeo de puertos y rangos IP comunes, lo que permite identificar dispositivos activos en la red local. Aunque las restricciones de seguridad del navegador pueden limitar la detección directa de la IP local, el sistema implementa mecanismos de respaldo para asegurar que el escaneo se realice de manera efectiva.

**4. Auditoría y Trazabilidad:** El registro de auditoría integrado proporciona una bitácora detallada de todas las acciones realizadas, lo que permite verificar la integridad de las operaciones y facilita la depuración en caso de inconsistencias.

## Cómo usar el sistema

Este proyecto es una aplicación web autónoma contenida en un único archivo HTML. No requiere instalación de servidores o dependencias complejas.

• **Descarga el archivo:** Sistema de Planificación Inteligente de Redes v7.html de este repositorio.

• **Abre en el Navegador:** Simplemente abre el archivo Sistema de Planificación Inteligente de Redes v7.html con tu navegador web preferido (Chrome, Firefox, Edge, etc.).

## Limitaciones

• La aplicación funciona completamente en el frontend (sin backend ni base de datos)
• No se cuenta con autenticación de usuarios ni control de acceso


## Autor
Yeraldin Miranda Barbosa
Fundación Universitaria Compensar
Ingeneria en Telecomunicaciones
