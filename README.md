# ⌚📡 OpenWatch — Indy Open HamWatch

### Tu estación de radio en la muñeca.

![OpenWatch Concept](./openwatch-concept.png)

**OpenWatch / Indy Open HamWatch** es un proyecto abierto de la familia **Indy Open**, orientado a crear nuevas herramientas para radioaficionados utilizando el **LILYGO T-Watch S3**.

La idea es aprovechar su **ESP32-S3**, pantalla táctil, conectividad Wi-Fi/Bluetooth y radio **LoRa 433 MHz** para convertirlo en una plataforma portátil de experimentación para APRS, mensajería, telemetría, monitoreo y otras funciones relacionadas con radioafición.

> [!IMPORTANT]
> ## 🚧 PROYECTO EN DESARROLLO
>
> **OpenWatch / Indy Open HamWatch se encuentra actualmente en desarrollo activo.**
>
> Las características, pantallas, funciones e integraciones descritas en este repositorio representan la visión y los objetivos actuales del proyecto.
>
> ⚠️ **Las funcionalidades pueden cambiar, añadirse, modificarse o eliminarse durante el proceso de desarrollo y pruebas.**
>
> Algunas funciones mostradas en la documentación y material promocional son conceptos previstos y **pueden no estar implementadas todavía**.
>
> Si quieres seguir la evolución del proyecto, utiliza ⭐ **Star** y 👀 **Watch** en GitHub para recibir las próximas actualizaciones.

---

## 🚀 ¿Qué queremos hacer?

OpenWatch busca convertirse en una pequeña plataforma abierta para llevar herramientas de radioafición directamente a la muñeca.

Entre las funciones que estamos explorando se encuentran:

- 📡 Monitor APRS / APRS-IS
- 📻 LoRa 433 MHz
- 💬 Indy Open Messenger
- 📊 Monitor de Indy Open iGate
- 📍 Telemetría de nodos
- 🌡️ Visualización de sensores
- 📳 Alertas mediante vibración
- 🔊 Herramientas de audio
- 〰️ Entrenador CW / Morse
- 🦊 Fox Hunt mediante LoRa
- 📶 Información RSSI / SNR
- 📋 Registro de actividad
- 🌐 Wi-Fi
- 🔵 Bluetooth

Y seguramente aparecerán nuevas ideas durante el desarrollo.

---

## 💬 Indy Open Messenger

Una de las funciones principales que queremos desarrollar es un sistema de mensajería directa utilizando **LoRa 433 MHz**.

La intención es que OpenWatch pueda comunicarse con otros dispositivos compatibles con el ecosistema Indy Open.

```text
OpenWatch
    │
    │ LoRa 433 MHz
    ▼
OpenWatch
```

También:

```text
OpenWatch
    │
    │ LoRa 433 MHz
    ▼
Indy Open LoRa
    │
    ▼
LILYGO / ESP32
```

El objetivo es crear un protocolo abierto que pueda transportar información como:

- Indicativo
- Mensajes
- Telemetría
- Estado de batería
- RSSI
- SNR
- Información de nodos

Todo ello sin depender necesariamente de Internet o de una red celular.

---

## 📡 APRS

Cuando exista conexión Wi-Fi, OpenWatch podrá explorar funciones relacionadas con **APRS / APRS-IS**.

Entre los objetivos se encuentran:

- Monitor de estaciones
- Visualización de últimas tramas
- Mensajes APRS
- Alertas dirigidas al usuario
- Estado de Indy Open iGate
- Información de actividad de red

Ejemplo conceptual:

```text
XE3ABC-7
> Indy Open iGate

Última trama: 20 s
Estado: ONLINE
```

---

## 🖥️ Pantallas previstas

La interfaz está pensada para aprovechar la pantalla táctil del T-Watch S3.

### 🏠 Inicio

Estado general del sistema:

- Indicativo
- Hora
- Batería
- Wi-Fi
- APRS
- LoRa
- iGate
- Mensajes pendientes

### 📡 APRS Monitor

Visualización de estaciones y actividad APRS.

### 📻 LoRa 433

Nodos LoRa cercanos e información de señal.

### 💬 Messenger

Mensajes directos entre estaciones compatibles.

### 🛰️ iGate Status

Estado de un equipo **Indy Open iGate** disponible en la red.

### 🌡️ Sensores

Información ambiental o telemetría recibida desde otros nodos.

---

## 🔧 Hardware objetivo

El desarrollo inicial está pensado para:

### LILYGO T-Watch S3

Características que queremos aprovechar:

- ESP32-S3
- LoRa SX1262
- 433 MHz
- Wi-Fi
- Bluetooth
- Pantalla táctil IPS 240 × 240
- RTC
- Acelerómetro BMA423
- Micrófono PDM
- Amplificador de audio MAX98357A
- Motor háptico
- USB OTG
- Gestión integrada de batería

---

## 🦊 Ideas futuras

OpenWatch pretende ser una plataforma experimental y abierta.

Algunas funciones que podremos investigar posteriormente:

- Fox Hunt LoRa
- Balizas
- Entrenador Morse
- Generador CW
- Notas de voz
- Telemetría
- Mapas simplificados
- Alertas APRS
- Comunicación con Indy Open LoRa
- Control remoto de Indy Open iGate
- Herramientas para POTA / SOTA
- Diagnóstico de enlaces LoRa

---

## 🌎 Parte de la familia Indy Open

OpenWatch forma parte de la familia:

- 📡 **Indy Open APRS**
- 🔧 **Indy Open TNC**
- 📻 **Indy Open LoRa**
- ⌚ **Indy Open HamWatch**

El objetivo común es desarrollar herramientas abiertas para experimentar, aprender y aportar nuevas ideas a la comunidad radioaficionada.

---

## 🧪 Estado del proyecto

🚧 **EN DESARROLLO ACTIVO**

OpenWatch se encuentra actualmente en sus primeras etapas.

Estamos definiendo y probando:

- Arquitectura del firmware
- Interfaz gráfica
- LoRa 433 MHz
- Indy Open Messenger
- Integración APRS / APRS-IS
- Conectividad Wi-Fi
- Integración con Indy Open iGate
- Comunicación con Indy Open LoRa
- Alertas y notificaciones
- Herramientas para radioaficionados

### ⚠️ Importante

La lista anterior representa nuestros objetivos actuales.

**Las funcionalidades finales pueden variar conforme avance el desarrollo.**

Durante las pruebas algunas características pueden ser modificadas, reemplazadas, ampliadas o descartadas.

Las imágenes y pantallas publicadas durante el desarrollo deben considerarse **conceptos de diseño** y no necesariamente representan la versión final.

---

## ⭐ Sigue el proyecto

Si te interesa OpenWatch:

- ⭐ Dale una **Star** al repositorio
- 👀 Usa **Watch** para recibir actualizaciones
- 🍴 Haz **Fork** si quieres experimentar
- 💡 Comparte ideas y sugerencias
- 🐛 Reporta errores
- 🤝 Contribuye al desarrollo

Cada colaboración ayuda a que el proyecto siga creciendo.

---

## ☕ Apoya el proyecto

Indy Open es un proyecto comunitario desarrollado por interés en la radioafición, la experimentación y el software/hardware abierto.

Si OpenWatch te resulta interesante y quieres ayudar a continuar desarrollando, probando hardware y creando nuevas funciones, puedes apoyar voluntariamente el proyecto.

❤️ **Las donaciones son completamente opcionales.**

**Próximamente añadiremos aquí las opciones disponibles para apoyar el desarrollo.**

---

## ⚠️ Aviso

Este proyecto tiene fines educativos y experimentales relacionados con la radioafición.

El usuario es responsable de operar cualquier transmisor respetando la legislación aplicable, las frecuencias autorizadas, los límites de potencia y las condiciones correspondientes a su licencia.

---

## 📜 Open Source

OpenWatch nace con la intención de ser un proyecto abierto.

Queremos que cualquier radioaficionado pueda:

**aprender → experimentar → modificar → mejorar → compartir**

---

## 📡 Indy Open

### Innovación abierta para la comunidad radioaficionada.

**Tu radio. Tu red. Tu proyecto.**
