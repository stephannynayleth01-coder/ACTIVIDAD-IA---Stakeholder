# Análisis PESTEL: Sistema de Inventario y Mantenimiento para Laboratorio Académico

## Contexto del Proyecto
El laboratorio académico cuenta con computadores, sensores, dispositivos electrónicos y herramientas de uso frecuente por estudiantes y docentes. Actualmente presenta deficiencias en el control de inventario, trazabilidad de mantenimientos, gestión de préstamos y actualización del estado de los activos. 

El presente análisis PESTEL identifica los factores externos críticos que condicionan el diseño, arquitectura y reglas del sistema.

---

## 1. P - Político

### Factor 1: Políticas institucionales para la gestión de activos
* **Impacto en el sistema:** Define la lógica y reglas de negocio obligatorias. El software debe acoplarse a los reglamentos existentes para la autorización de préstamos, tiempos límite, sanciones, flujos de mantenimiento y procesos formales de baja de equipos.
* **Evidencia requerida:** Reglamento institucional de laboratorios, manual de procedimientos de inventario y políticas de préstamo.

### Factor 2: Prioridades institucionales de inversión tecnológica
* **Impacto en el sistema:** Determina el respaldo institucional para el desarrollo e implementación del proyecto. Garantiza la viabilidad de escalabilidad a largo plazo y la asignación de recursos para infraestructura.
* **Evidencia requerida:** Plan de desarrollo institucional, proyectos aprobados y rubros presupuestales asignados a laboratorios.

---

## 2. E - Económico

### Factor 1: Costos de mantenimiento y reparación de activos
* **Impacto en el sistema:** Justifica la necesidad del módulo de mantenimiento. El sistema debe calcular el ciclo de vida útil y registrar costos operativos (repuestos, garantías, soportes técnicos) para evaluar la rentabilidad de reparar vs. reemplazar un activo.
* **Evidencia requerida:** Histórico de facturas de reparación, registros de garantías y hoja de vida de equipos dañados.

### Factor 2: Costo de oportunidad por inactividad de equipos
* **Impacto en el sistema:** Condiciona la urgencia de alertas automáticas en el software. La indisponibilidad de sensores o computadores afecta las clases y proyectos; el sistema debe minimizar el tiempo de parada técnica.
* **Evidencia requerida:** Reportes de clases afectadas o retrasos en proyectos por falta de equipos operativos.

---

## 3. S - Social

### Factor 1: Flujo de interacción de estudiantes y docentes con los activos
* **Impacto en el sistema:** Dicta la usabilidad y los roles de usuario. Dado que los préstamos son dinámicos y de alta frecuencia, el sistema requiere interfaces ágiles (ej. escaneo rápido) para evitar cuellos de botella en la entrega y recepción.
* **Evidencia requerida:** Bitácoras actuales de préstamo, volumen de solicitudes diarias y caracterización de usuarios (docentes/estudiantes).

---

## 4. T - Tecnológico

### Factor 1: Infraestructura tecnológica y de red disponible
* **Impacto en el sistema:** Restringe la arquitectura del software (despliegue local vs. nube, servidor dedicado o compartido). Determina la disponibilidad de conectividad e infraestructura sobre la cual correrá la aplicación.
* **Evidencia requerida:** Ficha técnica de servidores locales, topología de red del laboratorio y características de los equipos cliente.

### Factor 2: Integración con dispositivos, sensores y hardware del laboratorio
* **Impacto en el sistema:** Obliga al sistema a considerar capacidades de integración (APIs, lectura de tags RFID, códigos QR o comunicación IoT) para registrar automáticamente el estado o presencia de los elementos electrónicos.
* **Evidencia requerida:** Hojas técnicas de los sensores/dispositivos y protocolos de comunicación soportados.

---

## 5. E - Ecológico

### Factor 1: Gestión y disposición de residuos electrónicos (RAEE)
* **Impacto en el sistema:** Exige un módulo de trazabilidad para equipos dados de baja. El sistema debe clasificar el hardware obsoleto o irreparable para cumplir con la ruta institucional de reciclaje y disposición segura de RAEE.
* **Evidencia requerida:** Política institucional de gestión ambiental y normativa de residuos electrónicos.

---

## 6. L - Legal

### Factor 1: Protección de datos personales (Habeas Data)
* **Impacto en el sistema:** Obliga a implementar controles de seguridad, encriptación y roles de acceso. Al almacenar información sensible de estudiantes y docentes (cédulas, correos, registros de responsabilidad), el sistema debe cumplir con la legislación de protección de datos.
* **Evidencia requerida:** Política institucional de tratamiento de datos personales y normativa legal vigente.

---

## Factores Críticos de Mayor Impacto (Resumen Ejecutivo)

Si se evalúan los condicionantes mínimos para la viabilidad del proyecto, los dos factores determinantes son:

1. **Político (Políticas institucionales):** Gobierna **qué debe hacer** el sistema y bajo qué reglas de negocio operará obligatoriamente.
2. **Tecnológico (Infraestructura e integración):** Gobierna **cómo y dónde** se construirá el sistema, definiendo sus límites técnicos y de arquitectura.
