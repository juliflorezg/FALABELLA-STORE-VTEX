# Falabella Store Theme

Este proyecto fue creado usando la plataforma VTEX IO, se creó un clon de la tienda [falabella.com](https://www.falabella.com.co) para los diferentes viewport/dispositivos (desktop, tablet y móvil)

## Vista previa

![vista previa de la tienda](./home-preview.png 'vista previa de la tienda, Falabella')

## Configuración

### Paso 1 - Configuración Básica

Ingrese a la [guía de configuración básica](https://vtex.io/docs/getting-started/build-stores-with-store-framework/1) y siga los pasos indicados.

Al finalizar la configuración debería tener la linea de comandos (CLI) de VTEX así como un workspace (espacio de trabajo) de desarrollo en el que pueda trabajar.

### Step 2 - Clonación del repositorio

[Clone](https://github.com/juliflorezg/FALABELLA-STORE-VTEX-IO) este repositorio en su equipo de trabajo para trabajar de manera local en el proyecto.

Luego, ingrese a la carpeta del proyecto usando su terminal.

### Paso 3 - Editar el archivo `manifest.json`

Ahora es necesario editar el archivo `manifest.json` en la raíz de su proyecto.

Una vez se encuentre en este archivo, deberá cambiar los valores para `vendor` y `name`. `vendor` es su cuenta de VTEX, en donde está trabajando y `name` es el nombre que le quiera dar a su tienda, por ejemplo:

```json
{
  "vendor": "itgloberspartnercl",
  "name": "store-theme-falabella"
}
```

### Paso 4 - Instalar aplicaciones requeridas

Para poder utilizar Store Framework y trabajar en el tema de su tienda, es necesario tener instalados `vtex.store-sitemap` y `vtex.store`.

Ejecute el comando `vtex list`, para comprobar si estas aplicaciones ya se encuentran instaladas.

Si no lo están, ejecute el siguiente comando para instalarlos: `vtex install vtex.store-sitemap vtex.store -f`

### Paso 5 - Desinstalar el tema predeterminado

Ejecutando vtex list, puede verificar si algún tema está instalado.

Es común tener ya instalado un `vtex.store-theme` cuando inicia el proceso de desarrollo frontend de su tienda.

Por lo tanto, si lo encuentra en la lista de aplicaciones, copie su nombre y utilícelo junto con el comando `vtex uninstall`. Por ejemplo:

```json
vtex uninstall vtex.store-theme
```

### Paso 6 - Ejecute un preview de la tienda

Ha llegado el momento de cargar todos sus cambios locales a la plataforma VTEX, para esto, verifique que se encuentra en el workspace de desarrollo que ha creado con anterioridad, esto lo puede hacer usando el comando `vtex whoami`.

Una vez se ha verificado que se encuentra en el workspace correcto, puede ejecutar el comando `vtex link` para enlazar su proyecto local con la plataforma.

Si el proceso fue exitoso, debería poder ver el siguiente mensaje en su terminal: `App linked successfully`. Luego, ejecute el comando `vtex browse` para poder levantar una ventana en el navegador y poder ver su tienda en ella.

Esto le permitirá ver los cambios aplicados en tiempo real, a través de la cuenta y el espacio de trabajo en el que está trabajando.

## Builders

```json
{
  "assets": "0.x",
  "docs": "0.x",
  "store": "0.x",
  "styles": "2.x"
}
```

## Dependencies

```json
{
  "vtex.store": "2.x",
  "vtex.store-header": "2.x",
  "vtex.product-summary": "2.x",
  "vtex.store-footer": "2.x",
  "vtex.store-components": "3.x",
  "vtex.styleguide": "9.x",
  "vtex.slider": "0.x",
  "vtex.carousel": "2.x",
  "vtex.shelf": "1.x",
  "vtex.menu": "2.x",
  "vtex.minicart": "2.x",
  "vtex.product-details": "1.x",
  "vtex.product-kit": "1.x",
  "vtex.search": "2.x",
  "vtex.search-result": "3.x",
  "vtex.login": "2.x",
  "vtex.my-account": "1.x",
  "vtex.flex-layout": "0.x",
  "vtex.rich-text": "0.x",
  "vtex.store-drawer": "0.x",
  "vtex.locale-switcher": "0.x",
  "vtex.product-quantity": "1.x",
  "vtex.product-identifier": "0.x",
  "vtex.product-specification-badges": "0.x",
  "vtex.product-review-interfaces": "1.x",
  "vtex.telemarketing": "2.x",
  "vtex.order-placed": "2.x",
  "vtex.stack-layout": "0.x",
  "vtex.tab-layout": "0.x",
  "vtex.responsive-layout": "0.x",
  "vtex.slider-layout": "0.x",
  "vtex.iframe": "0.x",
  "vtex.breadcrumb": "1.x",
  "vtex.sticky-layout": "0.x",
  "vtex.add-to-cart-button": "0.x",
  "vtex.store-image": "0.x",
  "vtex.modal-layout": "0.x",
  "vtex.store-link": "0.x",
  "vtex.store-icons": "0.x",
  "vtex.product-list": "0.x",
  "vtex.store-video": "1.x",
  "vtex.disclosure-layout": "1.x",
  "vtex.checkout-summary": "0.x",
  "vtex.product-price": "1.x",
  "vtex.overlay-layout": "0.x",
  "vtex.product-highlights": "2.x",
  "vtex.sandbox": "0.x"
}
```

## PeerDependencies

```json
{
  "vtex.mega-menu": "2.x",
  "vtex.wish-list": "1.x",
  "vtex.reviews-and-ratings": "3.x"
}
```

## Custom Apps (componentes que deben instalarse en la tienda)

```json
{
  "itgloberspartnercl.whatsapp-button": "0.x",
  "itgloberspartnercl.bullets-diagramation": "0.x",
  "itgloberspartnercl.add-to-cart-info": "0.x",
  "itgloberspartnercl.head-tag": "0.x",
  "itgloberspartnercl.custom-department-search": "0.x",
  "itgloberspartnercl.pdf-reader": "0.x",
  "itgloberspartnercl.quick-order": "0.x",
  "itgloberspartnercl.special-diagramation": "0.x"
}
```

## Contributors

1. [Julian Florez](https://github.com/juliflorezg/)
