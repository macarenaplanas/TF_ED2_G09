# Monitor de frecuencia cardiaca
>**Asignatura:** Electrónica Digital II  - Universidad Nacional de Córdoba
>
>**Profesor:** Marcos Blasco
>
>**Integrantes:**
> * Martina Bruno
> * Carolina Ottero 
> * Macarena Planas Montilla 
>   
---
## Descripcion general del proyecto
En este proyecto final de Electrónica Digital II, se desarrolló un monitor de frecuencia cardíaca que mide las pulsaciones del paciente en tiempo real y determina si se encuentra dentro de los valores normales. El sistema resuelve el riesgo de la demora en la atención médica de urgencia mediante un motor paso a paso que simula una bomba de infusión automatizada: si se detecta taquicardia, el motor gira a la izquierda para suministrar bisoprolol, y si se detecta bradicardia, gira a la derecha para administrar atropina.
Este dispositivo está dirigido al personal de salud y a unidades de cuidados intensivos que requieren un monitoreo constante y una reacción inmediata. Al automatizar la entrega de fármacos según la necesidad del paciente, funciona como un soporte vital crítico que minimiza los tiempos de respuesta ante crisis cardíacas.

### Alcances del Proyecto

**El sistema SÍ es capaz de:**
* Medir la frecuencia cardíaca en tiempo real mediante un sensor óptico, empleando filtrado por histéresis por software para evitar ruidos o falsas lecturas.
* Visualizar las pulsaciones por minuto (PPM) en tres displays de 7 segmentos multiplexados y transmitir los datos mediante comunicación serie (UART).
* Actuar automáticamente ante emergencias controlando un motor paso a paso que simula una bomba de infusión: medio giro a la izquierda ante taquicardia (dosificación de bisoprolol) o medio giro a la derecha ante bradicardia (dosificación de atropina).

**El sistema NO incluye (Fuera de alcance):**
* Almacenamiento local de datos históricos en tarjetas SD o memorias externas.
* Conectividad inalámbrica (Wi-Fi/Bluetooth) para enviar alertas a dispositivos móviles.

### Posibles Etapas Siguientes (Líneas Futuras)

* Migración a PCB: Trasladar el diseño actual desde la protoboard hacia un circuito impreso (PCB) optimizado y diseñado bajo normas de compatibilidad electromagnética para entornos médicos.
* Telemetría Inalámbrica: Implementar un módulo de comunicación para enviar alertas críticas directamente a un panel de monitoreo central en la estación de enfermería.
