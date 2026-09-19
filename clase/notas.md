# Registro de Trabajo en Clase - Taller 6

## Fecha de la sesión
16/09/2026

## Integrantes presentes
- Juan Pablo Luna Zuleta
- Alejandro Riveros
- Martín Ortega

## Actividades realizadas en clase

Trabajamos el caso base de GobData siguiendo los cinco pasos de la guía. Primero listamos los datos y procesos sensibles del portal (cédula, historial clínico, dirección, certificados digitales, trazabilidad de trámites) y le asignamos a cada uno la norma que le aplica: Ley 1581 para los datos personales, con tratamiento reforzado en salud, e ISO/IEC 27001 para control de accesos y auditoría.

La discusión más larga del equipo fue sobre la diferencia entre "Parcial" y "Brecha". Al principio queríamos marcar algunos ítems como incumplidos y listo, pero la plantilla solo admite dos estados, así que quedó claro que la brecha no se marca en el checklist sino que se documenta aparte, con su riesgo. Terminamos con 12 ítems evaluados, 7 en Cumple y 5 en Parcial, y esos 5 Parcial se convirtieron en las 5 filas de la hoja Brechas Identificadas.

La segunda decisión de modelado fue la priorización. Acordamos que el riesgo de la brecha y su prioridad no son lo mismo: la falta de mecanismo de revocatoria tiene riesgo Medio pero prioridad Alta, porque es una obligación legal directa y de bajo costo de implementación. Los dos riesgos Alto (continuidad y exportación manual sin DLP) quedaron también en prioridad Alta por impacto.

Herramientas: la plantilla oficial en Excel, la visualización HTML del repositorio para revisar la evidencia de cada ítem y el chat de Teams del equipo para repartir las tareas.

## Boceto inicial del modelo

Hoja `Checklist General` (12 ítems, columnas N° / Categoría / Criterio / Nivel / Evidencia / Recomendación) → filtrar los marcados Parcial → hoja `Brechas Identificadas` (Categoría / Brecha / Riesgo / Recomendación Prioritaria / Prioridad). Ver `clase/checklist-gobdata.xlsx`.

## Tareas definidas para complementar el taller

| Tarea asignada | Responsable | Fecha estimada |
|----------------|-------------|----------------|
| Checklist del cliente real (17 ítems) en `entrega/checklist-cliente.xlsx` | Juan Pablo | 17/09 |
| Tabla de brechas priorizadas del cliente | Alejandro | 17/09 |
| Redacción del informe `entrega/informe.md` | Juan Pablo | 18/09 |
| Investigación normativa sectorial y `entrega/referencias.md` | Martín | 18/09 |
| Revisión final contra la checklist de autoevaluación de la guía | Equipo | 18/09 |

---

_Este documento resume el trabajo colaborativo realizado durante la sesión del Taller 6 en el curso AREM - Universidad de La Sabana._
