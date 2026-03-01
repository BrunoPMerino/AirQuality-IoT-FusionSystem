# 🌫️ ArduinoUno-AirQuality-FusionSystem

## 📌 Descripción del Proyecto

Este proyecto consiste en el diseño e implementación de un prototipo embebido IoT de bajo costo para el monitoreo en tiempo real de la calidad del aire en la región Sabana Centro (Cundinamarca, Colombia).

El sistema integra múltiples variables ambientales críticas y aplica lógica de fusión de datos para generar alertas tempranas **in situ**, sin utilizar redes de comunicación, cumpliendo con las restricciones técnicas del reto académico.

El sistema está desarrollado utilizando un **Arduino Uno** como microcontrolador principal.

---

## 🎯 Objetivo

Diseñar e implementar un sistema embebido capaz de:

- Medir material particulado (PM2.5 / PM10)
- Detectar gases contaminantes
- Registrar variables meteorológicas (temperatura, humedad y presión)
- Integrar múltiples señales mediante lógica de fusión ambiental
- Generar alertas locales en tiempo real mediante actuadores físicos

---

## 🧠 Arquitectura del Sistema

El sistema se compone de tres subsistemas principales:

### 1️⃣ Capa de Sensado
- PMS5003 → Material particulado (UART)
- MQ135 → Concentración de gases (Entrada analógica)
- BME280 → Temperatura, Humedad y Presión (I2C)

### 2️⃣ Capa de Procesamiento
- Arduino Uno
- Módulo de adquisición de señales
- Filtrado y validación de datos
- Normalización de variables ambientales
- Motor de fusión de datos
- Clasificación por umbrales de calidad del aire

### 3️⃣ Capa de Actuación e Interfaz
- Pantalla LCD (visualización en tiempo real)
- Buzzer (alerta sonora)
- LED RGB (indicador visual del estado del aire)

---

## 🚫 Restricciones de Diseño

- No se permite el uso de Raspberry Pi
- No se permite el uso de redes de comunicación para generar alertas
- El sistema debe operar de manera completamente autónoma
- Las alertas deben ser exclusivamente físicas y visuales (in situ)

---

## 📊 Clasificación de la Calidad del Aire

El sistema calcula un índice compuesto de calidad del aire y lo clasifica en:

- 🟢 Bueno
- 🟡 Moderado
- 🟠 Dañino
- 🔴 Peligroso

Cada nivel activa patrones específicos de alerta visual y sonora.

---

## 🧪 Validación Experimental

Se realizaron pruebas controladas variando:

- Exposición a material particulado
- Presencia de gases (simulación con alcohol)
- Cambios en variables ambientales

Se verificó el comportamiento de la lógica de fusión y la activación correcta del sistema de alertas ante escenarios críticos.

---

## 🛠️ Hardware Utilizado

- Arduino Uno
- Sensor PMS5003
- Sensor MQ135
- Sensor BME280
- Pantalla LCD con interfaz I2C
- Buzzer activo
- LED RGB

---

## 👥 Integrantes

- Nombre 1
- Nombre 2
- Nombre 3

Curso: Internet de las Cosas  
Facultad de Ingeniería  
Universidad de La Sabana  
2026-1  

---

## 🎥 Video Demostrativo

[Insertar enlace al video en MS Teams]

---

## 📚 Documentación Técnica Completa

La documentación técnica completa del proyecto, incluyendo:

- Restricciones de diseño
- Arquitectura del sistema
- Diagramas de bloques
- Diagramas UML
- Diseño de la lógica de fusión
- Configuración experimental
- Resultados y análisis
- Declaración del uso de Inteligencia Artificial (si aplica)

se encuentra disponible en la sección **Wiki** del repositorio.

👉 [Ir a la Wiki]

---

## 📌 Estado del Proyecto

✔ Prototipo funcional  
✔ Lógica de fusión implementada  
✔ Sistema de alertas validado  
✔ Documentación técnica en desarrollo  

---
