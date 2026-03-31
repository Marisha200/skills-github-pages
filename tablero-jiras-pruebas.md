# Tablero de JIRAs para registro de pruebas

Este tablero sirve para **registrar el estado de pruebas por cada JIRA** (funcionales, regresión, UAT y evidencia).

## Cómo usarlo

1. Crear una fila por cada JIRA.
2. Actualizar el estado de pruebas en cada avance.
3. Adjuntar evidencia (link a video, capturas o reporte).
4. Marcar "Listo para QA" solo si cumple DoR/DoD de pruebas.

## Tablero

| JIRA | Título | Responsable dev | QA asignado | Ambiente | Estado dev | Estado QA | Tipo de prueba | Resultado | Evidencia | Fecha de prueba | Observaciones |
|---|---|---|---|---|---|---|---|---|---|---|---|
| PROY-101 | Login con SSO | Ana | Carlos | QA | En progreso | Pendiente | Funcional | Pendiente | - | 2026-03-31 | Definir casos borde |
| PROY-102 | Recuperar contraseña | Luis | Carla | QA | Listo para QA | En ejecución | Regresión | Falló | https://... | 2026-03-31 | Error en token expirado |
| PROY-103 | Exportar reporte PDF | Sofía | Marcos | Staging | Listo para QA | Aprobado | UAT | Aprobado | https://... | 2026-03-31 | Sin observaciones |

## Estados sugeridos

### Estado dev
- Pendiente
- En progreso
- Listo para QA
- Bloqueado

### Estado QA
- Pendiente
- En ejecución
- Aprobado
- Rechazado
- Bloqueado

### Tipo de prueba
- Funcional
- Regresión
- Integración
- UAT
- Smoke

## Variante por columnas (Kanban)

Si prefieren un tablero tipo Kanban en JIRA, usar columnas:

1. Backlog
2. En desarrollo
3. Listo para QA
4. En QA
5. Rechazado QA
6. Aprobado QA
7. Done

Y en cada issue agregar campos:
- QA asignado
- Ambiente
- Resultado QA
- Evidencia
- Fecha ejecución QA

---

> Tip: este archivo se puede copiar a Confluence o a la descripción del tablero en JIRA para estandarizar el seguimiento de pruebas.
