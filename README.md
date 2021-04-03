m- es una librería CSS/JS que facilita la maquetación de contenidos en la web de Movistar Colombia.

# Carrusel

Copia y pega la siguiente estructura para crear un carrusel con un banner:

```html
<div class="m-carousel">
    <div class="m-carousel__banner">
        <div class="m-carousel__block m-carousel__block--hero">
            <div class="m-carousel__text">
                Ingresa el copy secundario del banner
            </div>
            <div class="m-carousel__text">
                Ingresa el copy primario del banner y usa br <br>
                para añadir saltos de línea
            </div>
            <div class="m-carousel__block">
                <img class="m-carousel__bullet" src="" alt="">
            </div>
            <div class="m-carousel__block">
                <div class="m-carousel__block">
                    <a class="m-carousel__button">Botón 1</a>
                    <a class="m-carousel__button">Botón 2</a>
                </div>
                <span class="m-carousel__text m-carousel__text--extra-small">
                    Aplican términos y condiciones
                </span>
            </div>
        </div>
    </div>
</div>
```
------------
### Elementos de un carrusel

| Nombre | Clase |
| :------------ | :------------ |
| [Carousel](#carousel "Carousel") | m-carousel |
| [Banner](#banner "Banner") | m-carousel__banner |
| [Block](#block "Block") | m-carousel__block |
| [Text](#text "Text") | m-carousel__text |

------------

### Carousel

**&rsaquo; `m-carousel`** crea un carrusel.

* Debe contener únicamente `m-carousel__banner`.

**&rsaquo; `--small`** reduce la altura del carrusel y ajusta sus elementos.

**&rsaquo; `--debug`** habilita el modo debug.

------------

### Banner

**`m-carousel__banner`** crea un banner.

* Debe crearse como hijo inmediado de un `m-carousel`.

------------

### Bloque

**&rsaquo; `m-carousel__block`** crea un bloque.

* Debe crearse como hijo inmediado de un `m-carousel__banner`.

**&rsaquo; `--hero`** modifica el bloque para la inclusión exclusiva de *copys* primarios y secundarios.

* Debe contener únicamente `m-carousel__text` hasta un máximo de dos.

* Si existe un único `m-carousel__text` este será el copy primario.

```html
<div class="m-carousel__block">
  <div class="m-carousel__text">
      Copy primario
  </div>
</div>
```

* Si existen dos `m-carousel__text` el primero será el copy secundario y el segundo el primario.

```html
<div class="m-carousel__block">
  <div class="m-carousel__text">
      Copy secundario
  </div>
  <div class="m-carousel__text">
      Copy primario
  </div>
</div>
```

**&rsaquo; `--buttons`** modifica el bloque para la inclusión exclusiva de botones.

------------

#### Text

**&rsaquo; `m-carousel__text`** inicia un texto.

**&rsaquo; `--hero`** modifica un bloque para la inclusión exclusiva de *copys* primarios y secundarios.

**&rsaquo; `--buttons`** modifica un bloque para la inclusión exclusiva de botones.
