# 📌 Medición de interacciones con el menú

## Descripción

Para medir las interacciones de los usuarios con los distintos elementos de navegación del menú del sitio, se implementó un nuevo evento en el Data Layer llamado **menu\_click**

### **Alcance implementado**

El evento se dispara al hacer clic sobre:

* Ítems del menú principal (**nivel\_1**)
* Subcategorías o elementos del flyout (**nivel\_2** y niveles posteriores)
* Banners promocionales dentro del menú (**banner**)
* Botones o enlaces de acción tipo **"Ver productos"** (**cta**)

\
**Estructura enviada al Data Layer**

{% code overflow="wrap" lineNumbers="true" expandable="true" %}
```
dataLayer.push({  
event: 'menu_click',  
menu_level: '',  
menu_item: '',  
menu_parent: '',  
menu_url: '',  
menu_creative: ''});
```
{% endcode %}

**Parámetros relevados**

| Parámetro       | Descripción                                                                                 |
| --------------- | ------------------------------------------------------------------------------------------- |
| `menu_level`    | Identifica el tipo de elemento clickeado (`nivel_1`, `nivel_2`, `nivel_3`, `banner`, `cta`) |
| `menu_item`     | Nombre visible del elemento seleccionado                                                    |
| `menu_parent`   | Categoría padre (cuando corresponde)                                                        |
| `menu_url`      | URL de destino                                                                              |
| `menu_creative` | Identificador o descripción del banner (solo para banners)                                  |

#### **Consideración para banners**

Para que el parámetro **`menu_creative`** informe correctamente el identificador del banner, es necesario que el equipo de contenido cargue un valor en el campo **"Texto alternativo de la imagen"** dentro del Site Editor. \
Dicho valor será utilizado como ID/descripción del banner al momento del clic.

<figure><img src="https://asanausercontent.com/us1/assets/66032875349265/1215254767757866/852a22d07c76e0210869ee1b2fed7454?e=1780339434&#x26;v=0&#x26;t=MVnbCscaFfjQWPqWZZ2md7s0lXhMyNWIAGryVxNlvkg" alt=""><figcaption></figcaption></figure>

#### **Visualización GTM**

<figure><img src="../../.gitbook/assets/Captura de pantalla 2026-05-29 a la(s) 5.25.34 p. m..png" alt=""><figcaption></figcaption></figure>

