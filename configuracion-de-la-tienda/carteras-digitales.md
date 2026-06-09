# 🔧 Carteras digitales

## Descripción

Una cartera digital (también llamada ewallet) es un ambiente seguro donde se pueden almacenar datos bancarios y/o de tarjeta de crédito. Esta información se cifra en el sistema y, cuando es accedida por su dueño, puede usarse para realizar compras en internet.

Comprar con una cartera digital ofrece más seguridad para el usuario, ya que no necesita informar sus datos de pago en el momento de la compra. En vez de eso, el usuario se redirige al ambiente de la cartera digital, donde deberá pasar por etapas de autenticación.

Con la identidad confirmada y el medio de pago elegido, la compra vuelve al flujo normal y el pedido se completa. Algunas carteras digitales funcionan todavía como subadquirentes, permitiendo que incluso una persona que no tenga registro sea capaz de realizar la compra a través de su ambiente.

Son ejemplos de carteras digitales que pueden ser configuradas para la realización de pagos en su tienda VTEX: **Paypal**, **Mercado Pago**, **Google Pay**, entre otras.

### Pasos para la configuración

A continuación se muestra un ejemplo de cómo configurar una cartera digital:

1.  En el administrador de VTEX, ingresar a **Configuración de la tienda > Pagos > Carteras digitales** escriba **Carteras** en la barra de búsqueda en la parte superior de la página.<br>

    <figure><img src="../.gitbook/assets/4 (13).png" alt=""><figcaption></figcaption></figure>
2. Al ingresar, nos mostrará la opción de **Google Pay** y debemos seleccionar **Activar** para configurarla.&#x20;
3. Una vez hecho esto, Google Pay estará disponible en el checkout de tu tienda VTEX como nuevo medio de pago. La configuración puede demorarse alrededor de 10 minutos en aparecer en el checkout.

{% hint style="info" %}
Para utilizar Google Pay deben cumplirse los siguientes requisitos:

* Tener al menos una condición de pago activa configurada para tarjetas de crédito o débito con un adquirente, definiendo qué adquirente procesará el pago.
* Utilizar el Checkout VTEX en tu tienda.
{% endhint %}
