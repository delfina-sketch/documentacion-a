# 🔧 Condiciones de pago

## Descripción

Una condición de pago en VTEX define **cómo un cliente puede pagar**, permitiendo configurar métodos (tarjeta, débito, pagarés, etc), cuotas, intereses, y reglas especiales (ej. solo para ciertos productos o categorías).&#x20;

En la práctica, las condiciones de pago son las opciones que aparecen en la pantalla del usuario al momento de finalizar la compra.

### Componentes clave de una condición de pago

* **Medio de Pago:** Tarjeta de crédito, débito, pagaré, etc., generalmente asociada a un proveedor (Gateway).
* **Reglas de Cuotas:** Permite definir si es al contado o en cuotas, número de cuotas, y si hay intereses (aplicando intereses de VTEX o del proveedor).
* **Condiciones Especiales:** Permite aplicar reglas a situaciones específicas (Por ej. solo para tarjetas de un banco, un monto mínimo/máximo, o un tipo de producto).
* **Procesamiento:** Se debe configurar la captura del pago (automática o manual, tras antifraude) y la asociación con un proveedor de pagos.&#x20;

### Secuencia Lógica para Evitar Errores

El orden correcto de configuración en VTEX es jerárquico:

1. Proveedor de pago (Por ej. Mercado Pago, Payway, etc)
2. Método de pago (Por ej. Tarjeta de crédito, débito, pagaré, etc)
3. Condición de comercial (Por ej. 3 cuotas sin interés, Ahora12, etc)

### Pasos para la configuración

1. En el Admin VTEX, accede a **Configuración de la tienda > Pago > Configuración**, o escribe **Configuración** en la barra de búsqueda en la parte superior de la página.
2. En la pestana **Condiciones de pago**, haga clic en el botón **+**.<br>
3. Una vez definido el proveedor, para elegir cualquiera de las condiciones de pago, siempre vas a necesitar:
   1. Rellenar el campo **Nombre de la regla** con un nombre de su elección para su identificación.
   2. Activar la condición en el campo **Status**.
   3. Indicar en **Procesar con proveedor**, qué proveedor tramitará esta condición de pago.
   4. Definir si desea utilizar un sistema antifraude en **Utilizar antifraude**.

Además, hay la posibilidad de definir si el pago será al contado o en cuotas, con o sin intereses y las condiciones especiales.

{% hint style="warning" %}
Cualquier cambio en las condiciones de pago puede llevar hasta 10 minutos en aparecer en el checkout de su tienda.
{% endhint %}

En los pasos siguientes, utilizaremos la tarjeta de crédito como ejemplo de condición de pago.

#### Al contado

1. En el Admin VTEX, acceder a **Configuración de la tienda > Pago > Configuración**, o escribir **Configuración** en la barra de búsqueda en la parte superior de la página.
2. En la pestaña **Condiciones de pago**, haga clic en el botón **+**.
3. Eligir el medio de pago tarjeta de crédito.
4. Rellenar el campo **Nombre de la regla** con un nombre de su elección para su identificación.
5. Activar la condición en el campo **Status**.
6. En el campo **Procesar con proveedor**, elija el proveedor que configuró (Importante: Antes de activar la condición de pago, comprobar con el gateway o adquirente si la bandera / medio de pago está disponible en su sistema).
7. Si desea utilizar un sistema antifraude, seleccione la opción **Utilizar antifraude**.
8.  En el campo ¿**Pago al contado o en cuotas?**, seleccione **Al contado**.<br>

    <figure><img src="../.gitbook/assets/image (272).png" alt=""><figcaption></figcaption></figure>
9. Haga clic en **Guardar**.

#### Cuotas sin interés

1. En el Admin VTEX, accedeR a **Configuración de la tienda > Pago > Configuración**, o escribir **Configuración** en la barra de búsqueda en la parte superior de la página.
2. En la pestaña **Condiciones de pago**, hacer clic en el botón **+**.
3. Eligir el medio de pago tarjeta de crédito.
4. Rellenar el campo **Nombre de la regla** con un nombre de su elección para su identificación.
5. Activar la condición en el campo **Status**.
6. En el campo **Proceso con proveedor**, elegir el proveedor que configuraste.
7. Si deseas utilizar un sistema antifraude, seleccione la opción **Utilizar antifraude**.
8. En el campo ¿**Pago al contado o en cuotas?**, seleccione **En cuotas**.
9. Configure el número de cuotas secuenciales (ej.: 1-10) o individuales (ej.:1,3,6), en el campo **Número total de cuotas**.
10. Defina una cuota mínima, para que sea aplicada conforme el valor de cada producto.
11. El campo **Facturación** sólo se tendrá en cuenta para cuotas que devenguen intereses, por lo que cualquier opción es válida.<br>

    <figure><img src="../.gitbook/assets/image (270).png" alt=""><figcaption></figcaption></figure>
12. Haga clic en **Guardar**.

#### Cuotas con interés

1. En el Admin VTEX, accedeR a **Configuración de la tienda > Pago > Configuración**, o escribir **Configuración** en la barra de búsqueda en la parte superior de la página.
2. En la pestaña **Condiciones de pago**, hacer clic en el botón **+**.
3. Eligir el medio de pago tarjeta de crédito.
4. Rellenar el campo **Nombre de la regla** con un nombre de su elección para su identificación.
5. Activar la condición en el campo **Status**.
6. En el campo **Proceso con proveedor**, elegir el proveedor que configuraste.
7. Si deseas utilizar un sistema antifraude, seleccione la opción **Utilizar antifraude**.
8. En el campo ¿**Pago al contado o en cuotas?**, seleccione **En cuotas**.
9. Configure el número de cuotas secuenciales (ej.: 1-10) o individuales (ej.:1,3,6), en el campo **Número total de cuotas**.
10. Defina una cuota mínima, para que sea aplicada conforme el valor de cada producto.
11. En **Facturación**, seleccionar la fecha de facturación con el inicio o fin del período (valor utilizado para calcular el monto de la cuota que devenga intereses).
12. Haga clic en **Establecer tasa de interés**.
13. En **Interés(%)**, digite el valor del interés que desea si aplicado a cada una de las cuotas. El campo permite agregar valores con hasta 2 decimales (por ejemplo, `1,25` y `10,89` son valores posibles).
14. Para elegir entre interés compuesto e interés simple, haga clic en **Se aplicó el interés compuesto > Cambiar**. Aparecerá una casilla de verificación que ofrece ambas opciones.<br>

    <figure><img src="../.gitbook/assets/image (269).png" alt=""><figcaption></figcaption></figure>
15. Haga clic en **Guardar**.

#### Eliminar condición de pago

1. En el Admin VTEX, acceder a **Configuración de la tienda > Pago > Configuración**, o escribir **Configuración** en la barra de búsqueda en la parte superior de la página.
2. En la pestana **Condiciones de pago**, haga clic en el condición de pago que desea eliminar.
3. Haga clic en el icono de la papelera.

<figure><img src="../.gitbook/assets/image (268).png" alt=""><figcaption></figcaption></figure>

