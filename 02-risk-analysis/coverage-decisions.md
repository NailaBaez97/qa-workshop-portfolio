# Coverage Decisions 
## Riesgos que se probarán primero 
1. El sistema podría procesar un pago exitoso pero no reflejar la compra en el sistema.
2. El carrito podría no actualizar correctamente la cantidad o el total de productos.
3. Los datos personales del usuario podrían ser expuestos en la aplicación.
## ¿Por qué esos riesgos son prioridad? 
Estos riesgos se priorizan debido a que impactan directamente en el flujo de compra y en la generación de ingresos del negocio. Además, afectan la confianza del usuario y la seguridad de la información, lo cual es crítico para el funcionamiento del sistema.
## Qué se probará menos o quedará fuera por ahora 
* Funcionalidad de búsqueda de productos
* Proceso de inicio de sesión
## Justificación de exclusiones 
Estas funcionalidades no se priorizan en una primera etapa, ya que no impactan directamente en la finalización de la compra ni en la generación de ingresos. Sin embargo, serán consideradas en fases posteriores de testing.