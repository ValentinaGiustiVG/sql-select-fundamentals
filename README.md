# sql-select-fundamentals-
# Consultas Básicas SELECT — TechStore

## Preguntas

### 1. ¿Por qué es mala práctica usar SELECT * en producción?
**Impacto en el rendimiento:** Consultar todas las columnas transfiere datos innecesarios a través de la red, consumiendo más memoria y ralentizando los servidores.
**Mantenibilidad y estabilidad:** Si en el futuro la base de datos suma o elimina columnas, las aplicaciones o reportes que dependen de un `SELECT *` pueden fallar inesperadamente por cambios en el orden o tipo de datos.

### 2. ¿Por qué son importantes los alias para un stakeholder no técnico?
Los alias sirven como traductor entre los nombres técnicos de la base de datos y el lenguaje de negocio.

**Ejemplo:** Una columna llamada `total_amount` resulta técnica e impersonal. Al renombrarla como `monto_total` o `ingresos_totales`, un analista de finanzas comprende de forma inmediata el valor del reporte en Excel o Power BI sin necesitar conocimientos de SQL.
