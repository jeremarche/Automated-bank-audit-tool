# Automated Bank Audit Tool 🏦🔍

Prototipo de herramienta de auditoría interna automatizada desarrollada en Python, diseñada para simular y analizar libros mayores contables, detectando anomalías, desvíos y posibles riesgos de fraude o ciberseguridad en el sector financiero.

## 🚀 Características principales
* **Detección de descuadres contables:** Identifica errores de tipeo o partidas desbalanceadas entre el Debe y el Haber.
* **Control de Caja Chica:** Detecta movimientos inusualmente altos o sospechosos en cuentas de efectivo menor.
* **Análisis de riesgos operativos (Horarios no hábiles):** Filtra transacciones realizadas fuera del horario laboral estándar, asociadas a riesgos de seguridad o accesos no autorizados.
* **Detección de duplicidad:** Encuentra asientos con IDs de transacción repetidos.

## 🛠️ Tecnologías utilizadas
* **Python**
* **Pandas** (Manipulación y análisis de datos tabulares)
* **NumPy** (Generación de estructuras y datos simulados)

## ⚙️ Cómo ejecutar el proyecto

1. **Generar los datos de prueba:**
   Ejecutá el script generador para crear el archivo del libro mayor simulado (`transacciones_banco.csv`):
   ```bash
   python generador_datos.py

## 📊 Ejemplo de Informe Generado (Output)
Cuando el script procesa el libro mayor, devuelve automáticamente un reporte como el siguiente:

```text
--- INFORME DE AUDITORÍA INTERNA AUTOMATIZADA ---
Archivo analizado: transacciones_banco.csv
Total de transacciones revisadas: 500

[!] Alerta 1: Se encontraron 4 posibles errores o descuadres contables:
[!] Alerta 2: Se encontraron 4 movimientos sospechosos en Caja Chica (montos excesivos):
[!] Alerta 3: Se detectaron 5 transacciones fuera de horario laboral (Riesgo de seguridad/fraude):
[!] Alerta 4: Se detectaron 2 registros con IDs de transacción duplicados:
--- FIN DEL INFORME DE AUDITORÍA ---
