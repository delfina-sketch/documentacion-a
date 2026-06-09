# 📌 Comprar juntos

### Descripción <a href="#descripcion" id="descripcion"></a>

Este desarrollo permite mostrar en la ficha de producto, debajo de las imágenes del mismo, un bloque donde se sugieren productos adicionales, para comprar junto al que se está visualizando.

De esta forma se incentiva al usuario a llevar un producto extra al que se observa en ficha, obteniendo un descuento.

### Pasos para la configuración <a href="#pasos-para-la-configuracion" id="pasos-para-la-configuracion"></a>

1. Acceder al administrador de VTEX.
2.  Ingresar por **Storefront** → **Site Editor** y dirigirnos a la URL de alguna ficha de producto. <br>

    <figure><img src="../../.gitbook/assets/arr2.png" alt=""><figcaption></figcaption></figure>
3.  Al ingresar, debemos abrir el bloque PDP (Desktop o Mobile según cuál vayamos a editar) localizar el bloque llamado **PDP Llevar Juntos**, abrirlo e ingresar al llamado **Buy Together.**<br>

    <figure><img src="../../.gitbook/assets/arr3.png" alt=""><figcaption></figcaption></figure>
4.  Desde el componente podemos encender o apagar el componente desde el switch, y también modificar la leyenda que figurará como título sobre el componente.<br>

    <figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

### ¿De dónde tomará el componente, el producto para mostrar como sugerencia? <a href="#de-donde-tomara-el-componente-el-producto-para-mostrar-como-sugerencia" id="de-donde-tomara-el-componente-el-producto-para-mostrar-como-sugerencia"></a>

Se deberá crear una especificación a nivel producto llamada "Buy together" para cargar el SKU que se desea que figure como sugerencia.

<figure><img src="../../.gitbook/assets/arr1.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Dentro de la especificación se debe colocar el ID del SKU. El componente solo toma un ID, por lo que no se debería cargar más de uno.
{% endhint %}

### Promoción para visualizar el descuento <a href="#promocion-para-visualizar-el-descuento" id="promocion-para-visualizar-el-descuento"></a>

Además de cargar los productos que figurarán como sugerencia, se debe crear un promoción de tipo "Comprar Juntos" en Vtex. [Link Documentación](https://help.vtex.com/en/tutorial/buy-together--tutorials_323).&#x20;
