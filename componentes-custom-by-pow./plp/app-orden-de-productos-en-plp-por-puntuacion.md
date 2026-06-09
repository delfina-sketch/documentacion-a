# 📌 App: Orden de productos en PLP por puntuación

## Descripción

Se desarrolló una aplicación **custom en VTEX** que permite **reordenar productos en las categorías y colecciones** de forma intuitiva, según las necesidades de la marca (No aplica dentro de departamentos). Esta mejora aplica tanto para **desktop como para mobile** y permite que el ordenamiento definido por la marca se refleje automáticamente en la PLP de productos correspondiente.

👉 La app se encuentra dentro del Admin de VTEX en: **Storefront > Custom app > Orden Gallery**

#### Funcionalidades principales <a href="#funcionalidades-principales" id="funcionalidades-principales"></a>

* Reordenar productos de **categorías** o **colecciones**.
* Mantener el ordenamiento definido, sin afectar los filtros estándar de la PLP (ventas, fecha de lanzamiento, precio, etc.).
* Administración sencilla a través de carga y actualización de archivos **CSV**.
* Descarga de plantillas de ejemplo para agilizar el proceso.
* Edición de registros ya creados, sin necesidad de cargar todo nuevamente.

#### Pantalla principal <a href="#pantalla-principal" id="pantalla-principal"></a>

Al ingresar a la app se encuentra una pantalla inicial con:

* **Videos explicativos**:
  * Cómo crear un CSV para el ordenamiento de la galería.
  * Cómo modificar un ordenamiento ya creado.

Estos recursos son útiles como guía rápida de uso.

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252FA9HraCbJNMR6ikaY7mQB%252Fimage.png%3Falt%3Dmedia%26token%3Dba8e343c-fb67-44da-9101-0c2e3186a5fb&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=a8136cfe&#x26;sv=2" alt=""><figcaption></figcaption></figure>

#### 📂 Sección de Creación de CSV <a href="#seccion-de-creacion-de-csv" id="seccion-de-creacion-de-csv"></a>

1. Seleccionar el botón CREAR
2. Se abrirá una nueva pantalla con el título: **Ordenamiento de galería, asignación de scoring**
3. Descargar el **CSV de ejemplo** disponible en la app (sirve como plantilla).

{% hint style="success" %}
Al descargar el archivo aparecerá un pop up en el borde superior derecho confirmando la descarga existosa del mismo.
{% endhint %}

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252FNCcQuCTQa3f3aZYUNefj%252Fprest1.png%3Falt%3Dmedia%26token%3D4ea7b163-65b8-461a-93d1-3a5e20208f06&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=37a6d046&#x26;sv=2" alt=""><figcaption></figcaption></figure>

4. **Completar el archivo** con los productos que se desean ordenar.

Como plantilla de ejemplo verán algo así:

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252Ftom4mvhGMRTlsKNbDVxX%252Fimage.png%3Falt%3Dmedia%26token%3D2799e965-0fbf-40c3-bfb0-e0c6feb4f817&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=480d75a2&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**A tener en cuenta:**

* Los **ID de productos** utilizados en los ejemplos son ficticios y se muestran solo a modo ilustrativo.
* El **scoring** (puntaje) indicado en los ejemplos también es de referencia.
* Se recomienda **iniciar siempre el ordenamiento con el scoring más alto** (se ordena de forma descendente, por lo que el mayor scoring se mostrará primero en la PLP)
* En la PLP de productos, **los items con menor scoring se mostrarán últimos**.
* El ordenamiento definido por la aplicación se mantiene **siempre que no se apliquen filtros del tipo `orderBy`** en la PLP (por ejemplo: ordenar por precio, fecha de lanzamiento o más vendidos).
*   En caso de que el usuario seleccione uno de estos filtros `orderBy`, prevalecerá el criterio elegido por el cliente final en la navegación, por encima del orden definido en la App.<br>

    <figure><img src="../../.gitbook/assets/image (201).png" alt=""><figcaption></figcaption></figure>

5\. En el **Paso 2** de la pantalla se debe seleccionar si el ID es de categoria o colección

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252FxiIfdO3rPqwYAKMxSKql%252Fimage%2520-%25202026-01-30T090013.878.png%3Falt%3Dmedia%26token%3D7b515f3d-d05a-486c-8b20-15a4fa772b7f&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=265e4dd&#x26;sv=2" alt=""><figcaption></figcaption></figure>

6. En el paso 3, debemos completar el ID de categoría o de colección:

* Ejemplo nombre de categoría: /ropadecama/sabanas
* Ejemplo ID de colección: `11`

7. En el **Paso 4** se debe **subir el CSV** previamente armado con los productos que se quiere ordenar.

Para ello se debe arrastrar el archivo y corroborar que luego figure como **"CSV cargado"** y con el nombre del archivo subido.

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252FIOYGNP5cngYVnWmqpF64%252Fimage.png%3Falt%3Dmedia%26token%3D788ad193-acb4-4062-902a-39b5a659a34d&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=1ad0b828&#x26;sv=2" alt=""><figcaption></figcaption></figure>

8. En el **Paso 5** el sistema hace un **conteo automático de los productos** cargados y crea el registro. Para finalizar seleccionar el botón **"Crear ordenamiento"**

Es importante verificar previamente los productos que figuran **a procesar** para asegurarse que se está tomando la cantidad total a ordenar en la PLP.

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252F7v50Ys7QUrMUkAv2kFm9%252Fimage.png%3Falt%3Dmedia%26token%3D883ec758-9635-4941-8a7a-a6e1c9c09f80&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=aa06a0b8&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**⚡Una vez guardado, el ordenamiento se aplica de manera automática en la PLP correspondiente.**

{% hint style="warning" %}
Información importante: Al cargar mas de un archivo con el mismo ID de ctaegoria y/o colección se va a agregar un Identificador asi saber cual fue el archivo que ser cargó primero:
{% endhint %}

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252F7CUBMl7jJCb7oUPWb0j1%252Fimage%2520-%25202026-01-30T090401.966.png%3Falt%3Dmedia%26token%3Da776b86f-f569-4584-a371-90710d252906&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=9078092e&#x26;sv=2" alt=""><figcaption></figcaption></figure>

No cargar .csv de forma consecutiva ya que por cada planilla se indexarán productos en categorías, lo cual creará inconsistencias en el catálogo hasta terminar la indexación.

#### 🔄 Sección de Modificación y/o búsqueda de CSV <a href="#seccion-de-modificacion-y-o-busqueda-de-csv" id="seccion-de-modificacion-y-o-busqueda-de-csv"></a>

Esta sección permite **gestionar y actualizar un ordenamiento ya creado**.

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252FE3KcCIVJOpDdeqtFR3Gf%252Fimage.png%3Falt%3Dmedia%26token%3Dc6575bc7-e58d-4690-a299-21d84e2f1248&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=6f7169ca&#x26;sv=2" alt=""><figcaption></figcaption></figure>

A tener en cuenta:

* **Entidad:** no es posible modificar ese campo
* **Campos:** dejar vacío (no se debe completar)
* **Tamaño de la página:** cantidad de filas que mostrará al hacer la búsqueda
* **Filtro (Where): Se coloca el nº de ID de categoría o colección específica que se desee buscar.**

En caso de no estar buscando algo en particular. Simplemente seleccionado el botón **"Buscar"** sin completar ningún campo, se listarán a continuación todos los ordenamientos creados y configurados en algún momento.

Al realizar una búsqueda o aplicar un filtro, se listan las categorías o colecciones que ya cuentan con un ordenamiento configurado. La tabla de resultados muestra la siguiente información de relevancia:

* **Acciones** → Columna con accesos rápidos:
  * **View** → permite visualizar el detalle del registro.
  * **Edit** → abre el modal de edición, donde se pueden hacer modificaciones (cambiar categoría, descargar plantilla, subir nuevo archivo).
  * **Delete** → elimina el registro del _master data_.
* **Category** → Indica la categoría o colección sobre la que se aplica el ordenamiento.
* **CreatedIn** → Fecha en la que se creó el registro.
* **UpdatedIn** → Fecha en la que se realizó la última actualización.

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252FxjzSHAiiEmEKKK9yG6RR%252Fimage.png%3Falt%3Dmedia%26token%3D9f2911d9-44d9-4ed9-9f20-d21d66e60c52&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=d4bb8d8a&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Si aparece con la leyenda **"null" en los último dos items mencionaos**, significa que el proceso no se completó correctamente y, probablemente, los cambios no se verán reflejados en el sitio (front).

**Al seleccionar EDIT** → abre un modal con más opciones:

* Cambiar el valor del campo **category:** de hacerlo el scoring definido para los productos aplicará en otra categoría (siempre y cuando los productos se encuentren ahi)

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252FQTKukQvWoGEunIXu79TX%252Fimage.png%3Falt%3Dmedia%26token%3Daaef208f-1fb7-4a88-b70c-3c789bd742ce&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=2e5cd8f5&#x26;sv=2" alt=""><figcaption></figcaption></figure>

* Descargar el registro actual en plantilla (útil si se necesita modificar un producto específico)

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252Fl0lzw38WAZTzGraN06k3%252Fimage.png%3Falt%3Dmedia%26token%3D25426032-47e4-424b-8f90-426c4ec004ab&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=27b218e1&#x26;sv=2" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Recomendación:** siempre descargar la plantilla antes de realizar cambios para contar con un respaldo en caso de errores.
{% endhint %}

* **Seleccionar archivo:** para subir el nuevo ordenamiento con los cambios aplicados

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252FQqnYZ5aEbFbGR37Fmjvc%252Fimage.png%3Falt%3Dmedia%26token%3Daa535975-71f1-41c9-aafa-0422edc14acb&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=a88e7a21&#x26;sv=2" alt=""><figcaption></figcaption></figure>

Figurará en verde una leyenda con la cantidad de productos leídos, cuando el archivo adjunto se haya cargado correctamente --> **"CSV procesado correctamente: x productos"**

* En caso de necesitar eliminar el archivo adjunto y cargar otro o corregir algo, está disponible el botón "LIMPIAR".

<figure><img src="https://pow-ecommerce.gitbook.io/vtex-prestigio/~gitbook/image?url=https%3A%2F%2F1512710426-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FCT78SEgzfUZ0pNHThmuW%252Fuploads%252Fx4FBVhXs2056jFk5j6iT%252Fimage.png%3Falt%3Dmedia%26token%3Dc60b62ce-d383-4f60-9762-5afe87a9fbb8&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=e3d382c4&#x26;sv=2" alt=""><figcaption></figcaption></figure>

**⚡ Una vez guardado, el ordenamiento se aplica de manera automática en la PLP correspondiente.**
