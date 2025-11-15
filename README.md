# Control-Digital  
### Prácticas de Control Digital con Controllino & HMI Stone

Este repositorio contiene una colección de **prácticas de laboratorio** orientadas al aprendizaje de **automatización**, **adquisición de datos**, **control digital** e integración con **HMI industriales**.  
Todo el contenido está diseñado con fines **educativos**, pero también puede servir como base para prototipos y aplicaciones en entornos reales.

---

## Contenido del Repositorio

| Proyecto | Descripción |
|------------|----------------|
| **Práctica 1 — Manejo de Salidas Digitales (Controllino Mega)** | Control de una matriz de LEDs 3×3 utilizando salidas digitales del Controllino Mega. |
| **Práctica 2 — Control Digital y Máquina de Estados (FSM)** | **A:** Uso de 3 botones para controlar LEDs. <br> **B:** Implementación de una máquina de estados para un semáforo simple. |
| **Práctica 3 — Interfaz Gráfica (HMI Stone)** | Control de encendido/apagado de LEDs y ajuste de brillo mediante una HMI STONE. |
| **Práctica 4 — Adquisición y Control PID de Motor DC** | Obtención de datos del encoder y control PID configurado desde la HMI. |

---

## Requisitos del Proyecto

### Hardware
- Controllino Mega  
- Pantalla HMI STONE (Serial TTL – 115200 baudios)  
- Motor DC con encoder (36 pulsos por revolución)  
- Fuente de alimentación para el motor  
- NI myDAQ  
- Kit EPC (si aplica)

### Software
- Arduino IDE  
- Librerías: `Stone_HMI_Define.h`, `Procesar_HMI.h`  
- NI LabVIEW (para simulaciones y obtención de la función de transferencia)

---

## Arquitectura General

```text
Controllino Mega
│
├── Sensores
│   ├── Encoder
│   └── Entradas Digitales
│
├── Actuadores
│   ├── LEDs
│   └── Motor DC
│
└── Interfaz HMI
    └── Comunicación Serial (UART)
