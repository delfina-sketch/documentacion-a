---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/72B6lE7Nn0jKtcyB10gI/modulo-de-catalogo/indexacion
---

# 👕 Indexación

{% hint style="danger" %}
**No se recomienda reindexar masivamente todo el catálogo de una vez**. El proceso de indexación es de a un producto a la vez, por lo que si forzamos el reindexado masivo de todo el catálogo podremos provocar que el indexador se cuelgue y todos los productos que estén pendientes no se reindexen hasta que se destrabe.

En el caso de indexar por carga masiva, se recomienda hacer, como máximo, de a un departamento por vez.
{% endhint %}

La indexación de productos es el proceso de organizar y registrar la información de los productos para que aparezcan correctamente en la tienda en línea. Esto ayuda a que los clientes encuentren fácilmente los productos y mejora la experiencia de compra.

Sin embargo, múltiples factores internos o externos pueden provocar que esta indexación no sea 100% exitosa en todos los productos, pudiendo provocar que uno o más artículos se visualicen de forma incorrecta (desactualizado) o que directamente no se visualicen. Por ello es importante saber que hay tres formas de forzado de reindexado. Están ordenadas de más leves a más agresivas:

## Indexar un producto manualmente

Para indexar un producto manualmente es necesario, primero, dirigirse al módulo de Todos los productos dentro de VTEX.

<figure><img src="../.gitbook/assets/41.png" alt=""><figcaption></figcaption></figure>

Una vez allí, debemos buscar el producto interesado en reindexar. Supongamos que es el Toallón Guarda Margaritas el que tiene problemas y que no impacta correctamente su precio, sus imágenes, o que simplemente más allá de cumplir todos los requisitos, aún no aparece en el sitio luego de un día.

En principio, es importante prestar atención la fecha de indexación. Esta fecha podemos visualizarla a simple vista desde la columna **Última actualización**

<figure><img src="../.gitbook/assets/42.png" alt=""><figcaption></figcaption></figure>

También podemos ver los detalles de la indexación, ingresando por los **tres puntitos > Ver detalles de indexación.**&#x20;

<figure><img src="../.gitbook/assets/43.png" alt=""><figcaption></figcaption></figure>

En este caso, se indica que la última vez en que se indexó el producto fue el 17 de Diciembre de 2025. Supongamos que hoy es 18 de Diciembre y que los cambios ya deberían estar impactados. En ese caso, haremos click a "**Editar producto**".

Ya dentro de las opciones para modificar el producto, haremos algún cambio que no sea significante en el producto (por ejemplo, sumar un espacio al final de la descripción del producto) para que nos aparezca la opción "**Guardar**" y le hacemos click.

<figure><img src="../.gitbook/assets/45.png" alt=""><figcaption></figcaption></figure>

De esta forma, sin necesidad de hacer ningún cambio estaremos forzando a VTEX a reindexar ese producto en específico, por lo que luego de, a mas tardar, 1 hora, ya debería tener la nueva fecha de indexación.

## Indexar más de un producto de forma masiva

Suponiendo que no es un único producto el que tiene problemas de indexación, sino una subcategoría, categoría o departamento enteros, es posible que el proceso de reindexado manual sea muy engorroso. Por ello, es posible también hacer una reindexación de forma masiva.

Es importante, no obstante, entender que el proceso de indexado es un producto a la vez. Esto quiere decir que, si de forma masiva colocamos todo el catálogo para reindexar, o por ejemplo, un departamento entero que contenga 2000 productos y 8000 SKUs, podríamos generar que el indexador se trabe y que todos los productos que hayan quedado en línea de espera no se indexen hasta que éste sea destrabado por el soporte de VTEX.

Por ello, se sugiere siempre ser mesurados con el reindexado masivo. Más vale ser precavido y reindexar de a un departamento o de a una categoría por vez, y asegurarse que no se comprometerá al catálogo.

Para forzar un reindexado masivo es necesario dirigirse al módulo [**Importación y exportación**](importacion-exportacion.md) y hacer click en la opción de Filtrar resultados o realizar una búsqueda.

<figure><img src="../.gitbook/assets/46 (1).png" alt=""><figcaption></figcaption></figure>

Allí se debe ir hasta Categoría y seleccionar la categoría deseada a reindexar. En este caso, utilizaremos el departamento Cocina.

<figure><img src="../.gitbook/assets/47 (1).png" alt=""><figcaption></figcaption></figure>

Hecho eso, exportaremos el catálogo en la sección de Exportación/Importación que está debajo de los filtros:

<figure><img src="../.gitbook/assets/48 (1).png" alt=""><figcaption></figcaption></figure>

Al exportarse, dará un mensaje donde se podrá descargar el departamento recién exportado. Ni bien descargado, debemos hacer click en Importar e importar el catálogo nuevamente sin realizar ninguna modificación ni edición del archivo. De esta forma nos aseguraremos que no estaremos realizando ningún cambio indeseado en productos, sino simplemente forzar la reindexación de todos esos productos.

<figure><img src="../.gitbook/assets/49.gif" alt=""><figcaption></figcaption></figure>

Hecho esto, podremos verificar desde los dos módulos que sirven para monitorear la indexación de productos. Uno en **Catálogo > Informes**.

<figure><img src="../.gitbook/assets/50 (1).png" alt=""><figcaption></figcaption></figure>

Y el otro, en **Storefront > Intelligent Search > Historial de indexación**

<figure><img src="../.gitbook/assets/51 (1).png" alt=""><figcaption></figcaption></figure>

## Reindexar toda la base

Este es el tipo más agresivo y complejo de los tres. Se utiliza únicamente en situaciones críticas en las que el reindexado masivo no genera resultados positivos y requiere de una medida más profunda.

En caso que todo el catálogo esté comprometido o el indexador esté trabado hace días, siempre es recomendable dar aviso a Pow. para que la situación se pueda evaluar y, en caso de ser necesario, en conjunto coordinar la reindexación de la base.
