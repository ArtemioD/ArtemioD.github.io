# artemiod.github.io

El sitio público de **[BiciBA](https://play.google.com/store/apps/details?id=com.artemiod.biciba)**,
servido en la raíz de `https://artemiod.github.io`.

`index.html` es la página entera: presenta la aplicación, muestra capturas y enlaza a la política de
privacidad, que vive en [PrivacidadBiciBa](https://github.com/ArtemioD/PrivacidadBiciBa). Sin
dependencias ni compilación, se abre tal cual.

## Por qué este repositorio existe en la raíz

Por **`app-ads.txt`**. Google AdMob lo exige para seguir publicando anuncios, y el estándar obliga a
servirlo en la **raíz del dominio** que figura como sitio web del desarrollador en la ficha de Google
Play: el rastreador pide `https://artemiod.github.io/app-ads.txt` y ninguna otra dirección. Una
subcarpeta no sirve, y por eso no pudo ir junto a la política.

Ya que el dominio raíz tenía que existir igual, aloja también la página del proyecto: es la
dirección que ve quien toca "sitio web del desarrollador" desde Play.

El `app-ads.txt` se actualiza solo si cambia el ID de editor de AdMob o si se suma otra red
publicitaria.
