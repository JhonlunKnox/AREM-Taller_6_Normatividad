# Taller 6: Checklist de Cumplimiento Normativo

## Objetivo

Verificar los aspectos legales, normativos y de cumplimiento que aplican al sistema del cliente, utilizando listas de control basadas en marcos como ISO 27001, GDPR, Habeas Data y la Ley 1581 de Protección de Datos en Colombia.

---

## Guía paso a paso

Antes de diligenciar el checklist, revise la [**Guía Paso a Paso: Checklist de Cumplimiento Normativo**](clase/guia_paso_a_paso_normatividad.md). Incluye un resumen de qué exige cada marco normativo, la metodología de 5 pasos (de identificar datos sensibles a recomendaciones priorizadas), un ejemplo completo construido paso a paso sobre el caso de GobData, y una tabla de errores comunes.

### Versión visual: Checklist de Cumplimiento Normativo

[`clase/visualizacion-normatividad.html`](clase/visualizacion-normatividad.html) es una página interactiva autocontenida: la matriz de los 12 ítems del checklist de GobData con su nivel de cumplimiento (Cumple / Parcial), un panel clickeable por ítem que muestra la evidencia real encontrada y la recomendación (y, si es un ítem Parcial, el riesgo y la recomendación prioritaria de la brecha derivada), la tabla derivada de Brechas Identificadas con su riesgo y prioridad, la metodología de 5 pasos y los errores comunes a evitar. GitHub no la renderiza interactiva desde la vista de archivo; para verla:
- Descargue el archivo y ábralo con doble clic (funciona sin conexión, es HTML plano), o
- Pegue esta URL en [htmlpreview.github.io](https://htmlpreview.github.io/): `https://raw.githubusercontent.com/CesarAVegaF312/AREM-Taller_6_Normatividad/main/clase/visualizacion-normatividad.html`

## Caso base de referencia: GobData (Portal de Trámites Ciudadanos)

GobData es un portal estatal donde los ciudadanos realizan trámites en línea relacionados con identidad, salud, impuestos, y derechos civiles. El sistema procesa grandes volúmenes de datos sensibles como números de identificación, historial clínico, direcciones y certificados digitales. Está sujeto a múltiples normativas nacionales como la Ley 1581 de Protección de Datos Personales, así como a estándares internacionales como ISO/IEC 27001. Evaluar el cumplimiento normativo permite garantizar la confianza del ciudadano y la integridad de los procesos públicos.

**Contexto:**
- GobData es una plataforma de atención digital del gobierno donde los ciudadanos pueden gestionar documentos, certificados, peticiones y notificaciones.
- Maneja información personal, datos sensibles (como historial médico o antecedentes), autenticación, trazabilidad y contacto con múltiples entidades públicas.

**Normativas a revisar:**

- Habeas Data (Ley 1581 de 2012 - Colombia)
- ISO/IEC 27001 (Gestión de Seguridad de la Información)
- Protección contra fugas de datos personales
- Consentimiento informado, auditoría, roles de acceso

---

## Parte 1: Trabajo en Clase

Durante la clase se espera que el equipo:

Siga la metodología de 5 pasos de la [guía paso a paso](clase/guia_paso_a_paso_normatividad.md) para evaluar el cumplimiento normativo de GobData:

1. Identifique los datos y procesos sensibles del sistema y la normativa aplicable a cada uno.
2. Construya el checklist agrupando los ítems por categoría (consentimiento, seguridad, protección de datos, prevención de fugas, retención).
3. Evalúe cada ítem como Cumple o Parcial, con evidencia; registre cada incumplimiento real como una fila en la tabla de Brechas Identificadas, con su riesgo.
4. Documente el riesgo legal u operativo de cada brecha.
5. Priorice las brechas y proponga una recomendación para cada una; valide con la [checklist de autoevaluación](clase/guia_paso_a_paso_normatividad.md#5-checklist-de-autoevaluación-antes-de-entregar).

- Registre brechas o hallazgos relevantes en `clase/checklist-gobdata.xlsx` y en `clase/notas.md` (use la [plantilla de notas](plantillas/plantilla_notas.md)).

---

## Parte 2: Aplicación al Cliente Real

Después de la clase, el equipo debe:

- Aplicar el mismo checklist al sistema del cliente, siguiendo los mismos 5 pasos de la metodología (`entrega/checklist-cliente.xlsx`).
- Indicar los elementos que cumplen y los que están en Parcial, registrando cada incumplimiento real en la tabla de Brechas Identificadas, con su riesgo y prioridad.
- Redactar el informe en `entrega/informe.md` usando la [plantilla de informe del taller](plantillas/plantilla_informe_taller.md), con recomendaciones concretas para cada brecha.
- Investigar normativas locales o sectoriales que impacten a su cliente (por ejemplo, MinSalud, MinTIC, SuperSalud, SFC), y registrar las fuentes en `entrega/referencias.md` con la [plantilla de referencias](plantillas/plantilla_referencias.md).

---

## Estructura esperada del repositorio

```text
taller-06-normatividad/
├── README.md
├── clase/
│   ├── guia_paso_a_paso_normatividad.md   # Marcos normativos, metodología de 5 pasos y ejemplo guiado
│   ├── checklist-gobdata.xlsx             # Checklist oficial (hojas Checklist General y Brechas Identificadas)
│   └── notas.md                           # Ver plantillas/plantilla_notas.md
├── entrega/
│   ├── checklist-cliente.xlsx
│   ├── informe.md                         # Ver plantillas/plantilla_informe_taller.md
│   └── referencias.md                     # Ver plantillas/plantilla_referencias.md
└── plantillas/
    ├── plantilla_checklist.xlsx           # Plantilla oficial en blanco, misma estructura que checklist-gobdata.xlsx
    ├── plantilla_informe_taller.md
    ├── plantilla_notas.md
    └── plantilla_referencias.md
```

---

## Errores comunes

Antes de entregar, compare su checklist contra los errores más frecuentes (ítems "Cumple" sin evidencia, confundir "Parcial" con "Brecha", recomendaciones sin relación con la brecha) documentados en la [sección 4 de la guía paso a paso](clase/guia_paso_a_paso_normatividad.md#4-errores-comunes-a-evitar).

## Entregables

- Checklist diligenciado para el cliente
- Informe técnico con hallazgos y recomendaciones
- Documento con referencias legales o normativas

---

## Rúbrica de Evaluación

| Criterio                            | Excelente (5)                                                            | Aceptable (3) / Insuficiente (1–2)                     |
|-------------------------------------|---------------------------------------------------------------------------|----------------------------------------------------------|
| Aplicación del checklist (caso base) | Diligenciado completamente con justificación técnica y legal             | Superficial o incompleto                                |
| Evaluación del cliente real          | Identifica brechas claras con impacto relevante                         | Generalizado o poco contextualizado                     |
| Informe y recomendaciones            | Presenta acciones correctivas viables según normativa                   | Recomendaciones vagas o sin fundamento                 |
| Investigación complementaria         | Uso adecuado de referencias legales y guías técnicas                    | Sin fuentes o referencias poco confiables               |

---

## Licencia

Este taller hace parte del curso de Arquitectura Empresarial - Universidad de La Sabana. Uso académico bajo licencia MIT.

---

## Entrega del equipo

| Archivo | Contenido |
|---|---|
| [`clase/notas.md`](clase/notas.md) | Registro del trabajo en clase sobre el caso base GobData |
| [`entrega/checklist-cliente.xlsx`](entrega/checklist-cliente.xlsx) | Checklist del cliente real: 17 ítems (6 Cumple / 11 Parcial) y 11 brechas priorizadas |
| [`entrega/informe.md`](entrega/informe.md) | Informe técnico con hallazgos, supuestos y recomendaciones |
| [`entrega/referencias.md`](entrega/referencias.md) | Referencias normativas y técnicas consultadas |

**Cliente:** Jefatura de Cultura de Innovación y Servicio - Universidad de La Sabana. Directorio de extensiones telefónicas (~6.400 registros) en Excel sobre OneDrive, operado por cuatro agentes de servicio.

**Equipo:** Juan Pablo Luna Zuleta, Alejandro Riveros, Martín Ortega.
