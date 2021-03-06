![](https://img.shields.io/static/v1?label=technology&message=css&color=blue)
![](https://img.shields.io/static/v1?label=technology&message=html&color=red)
![](https://img.shields.io/static/v1?label=school&message=udemy&color=red)


# CSSTransformsAndAnimations
Repositorio de ejemplos de CSS básico para las transformaciones de rotate, scale, skew, translate.

## Efectos en los botones
- Se ocupa los pseudo elementos `:before` y `:after`. Estos pseudo-elementos rellenan los botones con los efectos que deseamos.
- En el elemento se tiene que agregar overflow:hidden para que el pseudo-elemento solo se visualize dentro del elemento original
  `a { overflow:hidden; }`.

- `hover` debe aplicarse sobre el elemento y no sobre el pseudo-elemento
  `a:hover:before { }`.
  
- `transform` se utiliza para modificar el elemento en su posicion (`translate`), rotarlo(`rotate`), modificar su tamaño (`scale`).

- `transition` se utiliza en el elemento que no recibe el `:hover`, sirve para decir a que elementos se aplicará la animación y a que tiempo.

## Animaciones en CSS (animations)
- Para crear una animación, con solo *"dos etapas"* de animación, se hace lo siguiente:

```html
@keyframes nombreAnimacion {
  from {
    transform: translateX(0)
  }

  to {
    transform: translateX(100px)
  }
}
```

-Si quieres darle más etapas a la animación has lo siguiente:

```html
  @keyframes nombreAnimacion {
  0% {
    transform: translateX(0)
  }

  10% {
    transform: translateX(100px)
  }

  30% {
    transform: translateX(100px)
  }

  60% {
    transform: translateX(100px)
  }

  100% {
    transform: translateX(100px)
  } 
}
```

### Animación version corta (shorthand)
- version larga:

```html
div {
  animation-name: nombreAnimacion;
  animation-duration: 3s;
  animation-fill-mode: both;
  animation-iteration-count: infinite;
  animation-timing-function: ease-in;
  animation-direction: alternate;
  animation-delay: 1s;
}

@keyframes nombreAnimación {
  0% { transform: translateX(0) }
  50% { transform: translateX(50%) }
  100% { transform: translateX(100%) }
}

```

-- version corta
```html
div {
  animation: moving 3s both 3 ease-in alternate 1s;
}

@keyframes nombreAnimación {
  0% { transform: translateX(0) }
  50% { transform: translateX(50%) }
  100% { transform: translateX(100%) }
}

```
