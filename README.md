# Brazo Robótico Excavador TR4-G4M3 🤖🏗️

Este proyecto consiste en el diseño, construcción y control integral de un **brazo robótico no cartesiano** de tres grados de libertad, más un actuador final (pala), diseñado específicamente para la manipulación y transporte de arena mojada.

## 📋 Descripción General
El robot está inspirado en la morfología de una excavadora tradicional y se encuentra anclado a una base fija. El sistema es capaz de recoger material granular de una superficie plana y depositarlo en otra zona para generar un montículo, resolviendo la complejidad técnica de trabajar con materiales húmedos, pesados y de comportamiento semisólido.

## ✨ Características Principales
* **Diseño Integral desde Cero:** Modelado mecánico completo realizado en **Autodesk Fusion 360**.
* **Estructura Híbrida:** Combinación de eslabones de tubos cuadrados de aluminio y articulaciones de resina impresas en 3D de alta precisión.
* **Control de Lazo Cerrado:** Implementación de algoritmos **PID** (Proporcional-Integral-Derivativo) para garantizar la precisión en el posicionamiento de los motores.
* **Cinemática Avanzada:** Uso de modelos de cinemática directa e inversa (trigonométrica) para el cálculo de trayectorias en tiempo real.
* **Interfaz Móvil:** Aplicación Android personalizada desarrollada en **Kotlin** para el control remoto vía WiFi (TCP/IP).

## 🛠️ Especificaciones Técnicas

### Mecánica y Estructura
* **Grados de Libertad (DoF):** 3 ejes principales (Rotación de base/Swivel, Hombro/Pitch y Codo/Elbow) más el movimiento de la pala.
* **Transmisión:** Sistema de correas dentadas y poleas para optimizar el par y reducir la masa en movimiento.
* **Capacidad de Carga:** Diseñado para transportar entre 1 y 1.5 kg de arena mojada.
* **Área de Trabajo:** Operación eficiente en una superficie de al menos 20x20 cm.

### Electrónica
* **Controlador:** ESP32-WROOM-32 (Placa DevKit).
* **Actuadores:** Motores de corriente continua (DC) con reducción interna de 5 RPM y 10 RPM.
* **Sensores:** Encoders magnéticos de efecto Hall integrados para realimentación de posición.
* **Drivers:** Puente H L298N para el control de potencia y sentido de giro de los motores.
* **PCB Personalizada:** Diseño propio fabricado para integrar todos los componentes y minimizar el cableado.

## 💻 Software Utilizado
* **Modelado 3D:** Autodesk Fusion 360.
* **Programación Embebida:** Arduino IDE (C/C++).
* **Diseño de PCB:** KiCad.
* **Desarrollo Móvil:** Android Studio (Kotlin).

## 📊 Gestión del Proyecto
* **Presupuesto:** El costo total de ejecución fue de **133,84 €**, optimizando el uso de recursos frente al presupuesto máximo de 200 €.
* **Metodología:** Desarrollo basado en iteraciones de diseño 3D, fabricación por fases y validación de cinemática inversa.

## 👥 Integrantes del Equipo (T13-RR4)
* Jorge Moya Lucas
* Marcos Rodríguez Pena
* Alba Martínez Fernández
* Miguel Olalla Taladriz
* Paula Verdejo Rodríguez

---
*Este proyecto fue desarrollado bajo el marco académico de la Universidad Politécnica.*
