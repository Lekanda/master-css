<link href="style.css" rel="stylesheet"></link>

## Detalles Generales

- En *BS* hay 12 columnas para organizar los elementos.   
   
<img src="img/sizeBoot.png"></img>
> **Tabla de tamaños fijos en BootStrap**   
---

## Clases de BootStrap 4
> __Sustituir el *__    

|   **Clase**	|   **Explicacion**	|
|---	|---	|
|   **bg-***	|   Color de fondo de caja [Doc](https://getbootstrap.com/docs/4.6/utilities/colors/#background-color)	|
|   **p-***	|   padding [Doc](https://getbootstrap.com/docs/4.6/layout/utilities-for-layout/#margin-and-padding)	|
|   **w-***	|   Ancho en **%** de *1 a 100*	|
|   **col-lg-12**	|   *12* columnas de ancho max de *992px*	|
|   **justify-content-***	|   Alinea **horizontalmente**: **start, end, center, between, around**	|
|   **align-items-***	|   Alinea **verticalmente**: **start, end, center, between, around**	|
|   **align-self-start**	|   Alinea un *elemento* **verticalmente**: **start, end, center, between, around**	|
|   **order-**	|   Indica el orden:*1,2,3...*.Poner en todos	|
|   **offset**	|   Mete espacios en columnas. Info abajo.	|
|   **container-fluid**	|   Expande la caja al 100% de la pantalla.	|
|   	|   	|
|   	|   	|


<h2 class="subtitulo">Ancho automatico</h2>

- Hay que meter en cada **fila** en un *div* con clase **row**.   
- *Para ajustar los elementos*, poner **col** para ajuste automatico.   
    - **col-4** en un elemento da *4* de *mayor tamaño*.
```html
<section id="content" class="col-12">
            <div class="row">
                <section id="products" class="col-9 border">
                    <h2>Productos</h2>
                    <hr>
                    <div class="items">
                        <div class="row">
                                <div class="item col bg-primary m-2">
                                    Producto
                                </div>
                                <div class="item col bg-warning m-2">
                                    Producto
                                </div>
                                <div class="item col bg-success m-2">
                                    Producto
                                </div>
                        </div>
                        <div class="row mt-5">
                                <div class="item col bg-primary m-2">
                                    Producto
                                </div>
                                <div class="item col bg-warning m-2">
                                    Producto
                                </div>
                                <div class="item col bg-success m-2">
                                    Producto
                                </div>
                                <div class="item col bg-success m-2">
                                    Producto
                                </div>
                        </div>        
                    </div>
                </section>
                <aside id="barra" class="col-3 border">
                        <h2>Barra</h2>
                </aside>
            </div>
</section>
```



---
## Ejemplos de maquetacion

```html
<section id="content" class="col-12">
    <div class="row">
        <section id="products" class="col-9 border">
            <h2>Productos</h2>
        </section>
        <aside id="barra" class="col-3 border">
            <h2>Barra</h2>
        </aside>
    </div>
</section>
```   
> Maquetacion de *contenido* y *barra lateral*.    
---    


## Clase de Bootstrap Offset

- Es para *meter espacios en las columnas*. Hacemos que una columna sea un **espacio**.

> Se debe poner en el elemento de la **drch** *donde se quiere poner el espacio*.    



## Responsive en Bootstrap

- [Doc de Responsive Breakpoints](https://getbootstrap.com/docs/4.6/layout/overview/#responsive-breakpoints)   

- *Ejemplos*:
```html
    <li class="col-xs-12 col-sm-12 col-md">Inicio</li>

    <div class="item col col-lg col-md-12 col-sm-12 bg-primary">
        Producto
    </div>

    <aside id="barra" class="col-3 border d-none d-sm-none d-md-block">
```   

- *Puntos de corte.*   
```css
// Extra small devices (portrait phones, less than 576px)
// No media query for `xs` since this is the default in Bootstrap

// Small devices (landscape phones, 576px and up)
@media (min-width: 576px) { ... }

// Medium devices (tablets, 768px and up)
@media (min-width: 768px) { ... }

// Large devices (desktops, 992px and up)
@media (min-width: 992px) { ... }

// Extra large devices (large desktops, 1200px and up)
@media (min-width: 1200px) { ... }
```   

```html
    <nav id="menu" class="col-12 bg-secondary text-white d-none d-sm-none d-md-block">
```
