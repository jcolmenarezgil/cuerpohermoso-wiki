# Memoria y Reglas de Arquitectura - CuerpoHermoso Wiki

## Convención de Nomenclatura para Decisiones Arquitectónicas (ADR)

Todas las decisiones arquitectónicas, reglas técnicas y acuerdos de diseño deben seguir de manera uniforme el siguiente formato estándar:

* **Estructura:** `[PalabraClave] D-[000x]`
* **Reglas de Formato:**
  1. **Palabra Clave:** Identifica el área o módulo funcional correspondiente (ejemplos: `Finanzas`, `Servicios`, `Fotografias`, `Autenticacion`).
  2. **Identificador 'D-':** La letra `D` en mayúscula seguida obligatoriamente de un guion `-`.
  3. **Enumeración de cuatro dígitos:** Formato correlativo numérico con relleno de ceros a la izquierda `000x` (ejemplo: `0001`, `0002`, `0003`, ...).
  4. **Ejemplos válidos:**
     * `Finanzas D-0001`: Retención y depuración de comprobantes en Blob Storage.
     * `Finanzas D-0002`: Verificación criptográfica de pagos vía proveedor centralizado.
     * `Finanzas D-0003`: Cifrado a nivel de middleware para datos de pagadores (`payers`).
     * `Finanzas D-0004`: Vinculación obligatoria de pagos a activos/cuotas y planes de pago.
     * `Finanzas D-0005`: Desacoplamiento de fechas de agenda (`requestDay`) de la tabla de transacciones.
     * `Servicios D-0001`: Ciclo de vida y habilitación condicional de servicios médicos.
