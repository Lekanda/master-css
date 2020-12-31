##### Selector universal

- Seleccionas todo lo que hay en el DOM(etiquetas,clases,ids). 
```css
    *{
    color: rgb(155, 39, 39);
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    }
```    

##### Selector de Etiqueta

- Selecciona por etiqueta (h1,div,span, ...etc).
    - No se pone **nada**.     
```css
    h1{
        background: aqua;
    }
    a{
    font-size: 20px;
    color: brown;
    text-decoration: none;
    }
    /* Se selecciona el enlace a,   dentro del footer */
    footer a{
        color: cadetblue;
    }
```

##### Selector de Id

- Por **ID** se pone **#**.
- Se puede compartir una clase con varias: etiquetas,....etc
```css
    #descripcion{
        border: 2px solid black;
        padding:15px;
    }
    /* SE puede utilizar para mas de uno */
    #descripcion,
    #titulo{
    border: 2px solid black;
    padding:15px;
    }
```

##### Selector de Clase

- Selecciona por Clase. SE pone **.**.
```css

```



##### Selector de Atributo


