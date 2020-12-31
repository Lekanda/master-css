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
> Un *nombre de ID* solo se puede usar **una vez** en **un solo sitio**.        



##### Selector de Clase

- Selecciona por Clase. SE pone **.**.      
```css
    .parrafo{
    color: rgb(20, 45, 155);
    background-color: darkcyan;
    font-style: italic;
    text-decoration: underline;
    font-weight: bold;
}
```          
> Un selector de *clase* se puede usar **muchas** veces.
> Se puede usar varias clases para un mismo obj seleccionado.


##### Selector de Atributo

- Por el tipo de atributo que sea.   
```css
    /* Selector de atributo */
    #usuario form{
        border: 5px solid blue;
        margin-top: 15px;
        margin-bottom: 15px;
        padding: 15px;
    }
    #usuario form *{
        display: block;
    }
    /* Este es el ejemplo de por atributo */
    input[type="text"]{
        margin-bottom: 13px;
        padding: 6px;
        width: 300px;
    }
    input[type=submit]{
        background: green;
        color: greenyellow;
        font-weight: bold;
        font-size: 18px;
        text-transform: uppercase;
        border: 2px solid rgb(0, 63, 10);
        width: 150px;
        padding: 6px;
        cursor: pointer;
    }
```

##### Selector Hijo

- Para seleccionar poniendo la ruta exacta de lo que se quiere hacer.   
```css
/* Selector Hijo */
#menu > li > ul > li > a{
    font-size: 20px;
    color: rgb(247, 8, 8);
    text-decoration: none;
}

```      


##### Prioridad en CSS.

- CSS lee de arriba a abajo.   
- Cuanto mas especifica sea  una regla tiene mas prioridad.  
```css
    /* Prioridad */
        #saludo h1{
        background: blueviolet; 
        }
        h1{
            background: blue;
        }
```
> En este caso hara **#saludo h1**. Es mas especifica.

- Sí queremos que algo predomine por encima de los demas:    
```css
        h1{
            background: blue !important;
        }
```    
> **!important** hace que esa norma prevalezca por encima de las demas.

- Sí ponemos **!important** en varios , prioriza por las normas de antes.

