# artemiod.github.io

El sitio público de **[BiciBA](https://play.google.com/store/apps/details?id=com.artemiod.biciba)**,
servido en la raíz de `https://artemiod.github.io`. Sin dependencias ni compilación: las páginas se
abren tal cual.

| Ruta | Qué es |
|---|---|
| `/` | La página del proyecto: qué hace la aplicación, capturas y enlaces. |
| `/PrivacidadBiciBa/` | La política de privacidad, enlazada desde Google Play y desde la propia app. |
| `/app-ads.txt` | La declaración de AdMob. |

## Por qué todo vive acá

Por **`app-ads.txt`**. Google AdMob lo exige para seguir publicando anuncios, y el estándar obliga a
servirlo en la **raíz del dominio** que figura como sitio web del desarrollador en la ficha de Google
Play: el rastreador pide `https://artemiod.github.io/app-ads.txt` y ninguna otra dirección.

Ya que el dominio raíz tenía que existir igual, aloja también la página del proyecto —es lo que ve
quien toca "sitio web del desarrollador" desde Play— y la política de privacidad.

La política conserva a propósito la ruta `/PrivacidadBiciBa/`, que es la que quedó compilada dentro
de las versiones de la aplicación ya publicadas. Cambiarla dejaría ese enlace roto en los teléfonos
que no se actualicen.

## Mantener la política

Describe lo que la aplicación hace de verdad, así que **se actualiza junto con la app**: al agregar
un permiso, un SDK que procese datos o una función que guarde algo nuevo, hay que reflejarlo ahí y
cambiar la fecha de "Última actualización". Google Play compara lo que declara la ficha con lo que el
paquete realmente contiene.
