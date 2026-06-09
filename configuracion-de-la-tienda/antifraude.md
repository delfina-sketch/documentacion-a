# 🔧 Antifraude

## Descripción

Antifraude es un sistema especializado en analizar las compras realizadas en los sitios web, con el fin de identificar transacciones fraudulentas.

Recopila datos sobre el comportamiento de los usuarios y los compara con patrones sospechosos para aprobar o rechazar el pedido. De esta forma, la protección antifraude añade una capa adicional de seguridad a su tienda.

En VTEX, el operador de pagos primero aprueba la compra y luego el sistema antifraude evalúa el pedido. Si todo va bien, el proceso sigue su curso normal.

La plataforma VTEX está integrada con los siguientes sistemas antifraude:

* AcessoDigital
* Autentify
* B2eGroup
* Braspag
* ClearSale T
* ClearSaleGlobal
* ClearSaleV3
* CyberSource
* FUGU
* IG
* KoinAntifraud
* Konduto
* Kount
* Legiti
* Nethone
* RiskiedFraud
* Signifyd
* VestGuarantee

### Pasos para la configuración

1. En el administrador de VTEX, dirigirse a **Configuración de la tienda > Pago > Proveedores** o escribir **Proveedores** en la barra de búsqueda en la parte superior de la página.
2.  En la pantalla de proveedores, hacer clic en el botón **Nuevo proveedor**.<br>

    <figure><img src="../.gitbook/assets/5 (10).png" alt=""><figcaption></figcaption></figure>
3.  Escribir el proveedor antifraude deseado en la barra de búsqueda y hacer clic en su nombre.<br>

    <figure><img src="../.gitbook/assets/6 (8).png" alt=""><figcaption></figcaption></figure>
4.  Llenar los campos del formulario con los datos indicados por el proveedor antifraude.<br>

    <figure><img src="../.gitbook/assets/image (265).png" alt=""><figcaption></figcaption></figure>
5. Haga clic en **Guardar**.
6. Tras habilitar el proveedor antifraude, es necesario asociarlo con uno o más métodos de pago. Para ello, se deben seguir estos pasos:
   1. En el administrador de VTEX, acceder a **Configuración de la tienda > Pagos > Configuración** o escribir **Configuración** en la barra de búsqueda en la parte superior de la página.
   2.  En la pestaña **Condiciones de Pago**, hacer clic en el botón `+`.<br>

       <figure><img src="../.gitbook/assets/8 (8).png" alt=""><figcaption></figcaption></figure>
   3. Hacer clic en el método de pago deseado.
   4. Completar el campo **Nombre de la condición** con un nombre de su elección para su identificación.
   5. Activar la condición en el campo **Estado** .
   6. En **Proceso con proveedor** seleccionar el proveedor de pago deseado.
   7.  En **Usar solución antifraude**, seleccionar el proveedor antifraude habilitado previamente, si está disponible para su uso con este método de pago.<br>

       <figure><img src="../.gitbook/assets/9 (6).png" alt=""><figcaption></figcaption></figure>
7. Haga clic en **Guardar**.
