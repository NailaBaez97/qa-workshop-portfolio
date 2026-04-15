# Sesión 1

## Charter
Explorar el flujo completo de compra con el objetivo de identificar posibles fallos en la validación de datos, el cálculo de precios y la confirmación de pedidos.

## Áreas exploradas
- Catálogo de productos  
- Carrito de compras  
- Registro / Login  
- Proceso de checkout  
- Confirmación de orden  

## Inicio
**07/05/2026 - 13:00 hs**

## Tester
**Naila Baez**



## Desglose de tareas
-  10 min: Exploración de categorías y selección de productos  
-  10 min: Pruebas en el carrito (agregar, eliminar y actualizar cantidades)  
-  15 min: Intento de compra con usuario nuevo  
-  10 min: Validación con datos inválidos y escenarios límite  

---

## Archivos de datos
- Usuario nuevo (registro)  
- Datos de pago simulados  
- Entradas inválidas (campos vacíos, caracteres especiales, cantidades elevadas)  



## Notas de prueba
- La navegación por categorías y visualización de productos funciona correctamente.  
- La adición de productos al carrito se realiza sin inconvenientes.  
- El sistema bloquea correctamente el ingreso de cantidades negativas.  
- Se permite ingresar cantidades excesivamente altas sin restricciones visibles.  
- No se identifican validaciones claras para límites máximos de cantidad.  
- Durante el registro de usuario (requerido para comprar), el sistema arroja un error 500, impidiendo continuar.  
- Debido a este error, no fue posible completar el flujo de checkout.  



## Lista de riesgos
- Posible indisponibilidad en funcionalidades críticas (registro y checkout).  
- Riesgo de pérdida de ventas por fallos en el proceso de compra.  
- Posibles inconsistencias o sobrecarga por falta de límites en cantidades.  
- Experiencia de usuario negativa debido a errores no controlados (error 500).  


## Defectos (Bugs)
- **BUG 1:** El sistema devuelve un error 500 durante el registro de usuario, bloqueando la compra.  
- **BUG 2:** No existe un límite máximo definido al ingresar cantidades en el carrito.  
- **BUG 3:** Algunos productos presentan imágenes incorrectas o poco representativas.  
- **BUG 4:** Hay productos listados sin información clara sobre su disponibilidad en stock.  

---

## Incidentes (Issues)
- No se puede determinar si el error 500 corresponde a una falla temporal o a un problema persistente.  
- No se encuentran definidas reglas de negocio sobre límites de compra por producto.  
- No hay claridad sobre cómo se gestiona el stock desde la interfaz de usuario.  