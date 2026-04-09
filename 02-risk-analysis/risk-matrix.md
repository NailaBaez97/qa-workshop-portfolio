# Risk Matrix 
| ID | Riesgo | Impacto | Probabilidad | Nivel | Mitigación | 
|----|--------|---------|--------------|-------|------------| 
| R1 | El sistema permite continuar el proceso de compra de productos sin stock disponible. | 5 | 4 | 20 | Implementar validaciones de stock antes de permitir avanzar en el flujo de compra. | 
| R2 | El sistema permite ingresar cantidades inválidas (negativas o excesivas) en el carrito. | 5 | 4 | 20 | Validar los valores permitidos en la cantidad de productos y limitar según stock disponible. | 
| R3 | El sistema no permite a los usuarios autenticarse correctamente después del registro. | 5 | 3 | 15 | Validar el correcto funcionamiento del registro y login mediante pruebas funcionales y de integración. | 
| R4 | La funcionalidad de búsqueda no devuelve resultados consistentes ni proporciona retroalimentación clara al usuario. | 4 | 4 | 16 | Mejorar la lógica de búsqueda y mostrar mensajes claros cuando no se encuentren resultados. | 
| R5 | El sistema muestra mensajes de error técnicos (error 500) que no son comprensibles para el usuario. | 4 | 3 | 12 | Implementar manejo de errores con mensajes amigables y controlados para el usuario final. | 

## Justificación

* R1: Se asigna un impacto alto (5) debido a que permite realizar compras de productos sin stock, afectando directamente la operación del negocio. La probabilidad es alta (4) ya que el comportamiento fue observado directamente durante la prueba.

* R2: Se asigna un impacto alto (5) porque permite ingresar valores inválidos que afectan el cálculo del total de compra. La probabilidad es alta (4) ya que el sistema acepta estos valores sin validación.

* R3: Se asigna un impacto alto (5) porque impide que los usuarios accedan al sistema, bloqueando el proceso de compra. La probabilidad es media (3) ya que el fallo fue observado pero podría estar relacionado con el entorno de prueba.

* R4: Se asigna un impacto medio-alto (4) porque afecta la capacidad del usuario para encontrar productos, reduciendo la conversión. La probabilidad es alta (4) ya que se observaron inconsistencias en múltiples búsquedas.

* R5: Se asigna un impacto medio-alto (4) porque muestra mensajes técnicos que afectan la experiencia del usuario. La probabilidad es media (3) ya que ocurre en escenarios específicos como URLs inválidas.