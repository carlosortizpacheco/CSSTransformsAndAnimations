![](https://img.shields.io/static/v1?label=technology&message=css&color=blue)
![](https://img.shields.io/static/v1?label=technology&message=html&color=red)
![](https://img.shields.io/static/v1?label=school&message=udemy&color=red)


# CSSTransformsAndAnimations
Repositorio de ejemplos de CSS básico para las transformaciones de rotate, scale, skew, translate.

## Efectos en los botones
- Se ocupa los pseudo elementos `:before` y `:after`. Estos pseudo-elementos rellenan los botones con los efectos que deseamos.
- En el elemento se tiene que agregar overflow:hidden para que el pseudo-elemento solo se visualize dentro del elemento original
  `a {`
    `overflow:hidden;`
  `}`

- El `hover` debe aplicarse sobre el elemento y no sobre el pseudo-elemento

`a:hover:before {`
`}`
