---
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
metaLinks:
  alternates:
    - https://app.gitbook.com/s/72B6lE7Nn0jKtcyB10gI/modulo-de-precios/cupones
---

# 💸 Cupones

{% hint style="warning" %}
Desde Pow aconsejamos ante la habilitación del modulo Cupones, el exhaustivo, minucioso y periódico control de este bloque dado que la creación de un Cupón es estar creando dinero para utilizar en la web. Asimismo recomendamos la revisión de los perfiles y sus roles asignados para evitar y/o disminuir acciones que comprometan la integridad del sitio tanto como acciones mal intencionadas de terceros.

Lo aconsejable en este punto es que **solo un grupo muy reducido de perfiles** cuenten con acceso a este nuevo módulo.
{% endhint %}

## Cupones

Para crear un cupón de descuento, es necesario dirigirse al módulo **Promociones > Cupones**. \
Una vez allí, tendremos un listado de los cupones actuales y la opción de "Crear cupón". Le haremos click.

<figure><img src="../.gitbook/assets/5 (8).png" alt=""><figcaption></figcaption></figure>



## Uso del cupón y promociones asociadas

<figure><img src="../.gitbook/assets/3 (7).png" alt=""><figcaption></figcaption></figure>

Desde esta sección podremos ver tanto la cantidad de veces que se utilizó este cupón, como la cantidad y las promociones que están asociadas a este cupón.

{% hint style="info" %}
Para que el cupón funcione, sí o sí debe estar asociado a una promoción. Para ello, se puede crear directamente la promoción o asociarla manualmente. Para más información revisar[ Asociar cupón a promoción.](cupones.md#asociar-cupon-a-promocion)
{% endhint %}

## General

<figure><img src="../.gitbook/assets/4 (8).png" alt=""><figcaption></figcaption></figure>

En las configuraciones generales, tendremos en principio el código del cupón. Este código será el que tenga que ingresar el cliente, por lo que debe reflejar la intención del cupón. En el caso de generarse cupones en lote, será el prefijo de todos los códigos.

Ejemplo, si nuestro código del cupón es "Cupónprueba" y generamos en lote, los códigos podrán ser "Cupónprueba-15sgds56fa", "Cupónprueba-542fds54" y así.

Fuente UTM y Campaña UTM son parámetros de la URL para poder rastrear el alcance del cupón. Si bien no se necesitan ambas, es obligatorio tener al menos una configurada.

* **utm\_source:** el origen del tráfico, es decir, de qué sitio, anunciante o publicación vino el usuario.
* **utm\_campaign:** el nombre de la campaña que define determinado contexto de marketing (ejemplos: natal, lanzamiento, promo01).

La generación de cupones en lote permitirá que podamos tener distintos subcupones para el mismo cupón, y así poder diferenciar de repente dentro de un mismo cupón general, cual sí se usó y cual no, o poder repartir varios cupones que puedan utilizarse una sola vez. 1000 es el máximo permitido.

Al habilitar restricciones, estaremos limitando el uso de cada cupón.

## Restricciones

Al habilitar restricciones, estaremos limitando el uso de cada cupón. <br>

<figure><img src="../.gitbook/assets/image (182).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
Si se generan cupones en lote, la restricción aplica a cada subcupón de forma individual. Esto quiere decir que, si generamos 5 cupones en lote y asignamos una restricción de 2 usos máximos, cada cupón se podrá usar 2 veces, dando un total de 10 usos (Por ejemplo: 5 cupones X cada 2 usos = 10 total // 5 x 2 = 10).

Normalmente si se quiere generar un lote y que se utilice 1 vez cada uno, esta opción de restricción quedará en 1 máximo.
{% endhint %}

## Cupón generado

Una vez generado el cupón, en caso de haber activado la generación en lote, podremos entrar al cupón mismo y tendremos la posibilidad de copiar o exportar la **lista de cupones generados con su correspondiente código aleatorio.**

## Asociar cupón a promoción

Para que el cupón esté activo, es necesario asignarlo a una promoción existente o crear una. Para ello existen varias formas:

### Asociar a promoción existente

Si la promoción ya existe, vamos directamente a la promoción y asignamos el mismo UTM que hayamos aplicado en el cupón. Si por ejemplo, nosotros configuramos el UTM de campaña "promoprueba", vamos a la promoción que queramos asignar y colocamos el mismo UTM.

<figure><img src="https://lh7-us.googleusercontent.com/YlWyE3IexShn3y-iHSgOmsRtiC42g6HfGI0BRWA1deTJuI5XyRmR6pTmf7-DcGRSdaRWoyW-mWU89LpSY3U__Rr2-jAkzusbeo-Ids355ieSyLA4eR4Vwv7A6c4WFuOCAaabvJETk9-cD7-BjZDhAeg" alt=""><figcaption></figcaption></figure>

Al ir a la promoción y asignar el mismo UTM y tipo (no confundir UTM source y UTM campaign) ya nos dará la lista de códigos a las que aplica:<br>

<figure><img src="../.gitbook/assets/image (183).png" alt=""><figcaption></figcaption></figure>

### Crear promoción en base al cupón

Si no tenemos la promoción creada, desde el recuadro "-- promociones asociadas" podremos directamente crear la promoción:<br>

<figure><img src="../.gitbook/assets/5 (5).png" alt=""><figcaption></figcaption></figure>

Desde esta misma opción podremos crear directamente la promoción en base a nuestras necesidades para ese cupón especifico:

<figure><img src="../.gitbook/assets/6 (5).png" alt=""><figcaption></figcaption></figure>

### Crear cupón en base a la promoción

Si ya tenemos la promoción pero aún no tenemos el cupón, desde la misma pantalla de Promociones podremos crear un cupón en base a la UTM seleccionada.<br>

<figure><img src="../.gitbook/assets/7 (6).png" alt=""><figcaption></figcaption></figure>

De esta forma nos llevará directamente a la creación del cupón en base al UTM o los UTMs seleccionados en la configuración de la promoción.

<figure><img src="../.gitbook/assets/image (184).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Es posible utilizar en un cupón un utm source y un utm campaign al mismo tiempo.&#x20;

Lo que NO es posible es no utilizar ninguno, ya que requiere al menos uno.
{% endhint %}
