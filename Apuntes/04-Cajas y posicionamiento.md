### Cajas y Posicionamiento

#### Margenes, Padding, alto, ancho y bordes en CSS

- Nos quita los margenes y pading *prefijados en el div*
```css
*{
    margin: 0px;
    padding: 0px;
}
```

- Margin de : top, right,bottom,left
```css
    margin: 15px 15px 15px 15px
```    
- Se puede independientemente cada uno. CUIDADO: el individual debe ser mayor que el generico cuando estan los 2.

> **El div no varia su tamaño lo hace el padding, margin y border.**

> `margin: 0px auto;` => Centra el bloque


#### Posicionamiento de cajas

##### Float

- sirve para possicionar los **DIV**.
    - left,right,none,inline_start, inline_end.

##### Display

- Dice que comportamiento tiene que tener
    - **block**: Se comportan como bloques .Este es el mas normal.
    - **inline**:Se comporta como una linea de texto ->

> Para poder posicionar bien los enlaces y otros, se deben meter dentro de un *div*. **Si no, no deja**. Deja dimensionar pero no posicionar.

##### max-width

- Max tamaño de ancho       
`max-width: 1000px ;`     
> Igual con **min**.


##### clearfix

- En HTML ponemos el div , en el que no queremos que herede el flotante.
```html
    <!-- Limpiar los flotados -->
    <div class="clearfix"></div> 
```

- En CSS ponemos los estilos.
```css
.clearfix{
    float: none;
    clear: both;
}
```






