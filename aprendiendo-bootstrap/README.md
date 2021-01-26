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
|   **text-primary**	|   Color de texto.[Colores](https://getbootstrap.com/docs/4.0/utilities/colors/#color)	|
|   **p-***	|   padding [Doc](https://getbootstrap.com/docs/4.6/layout/utilities-for-layout/#margin-and-padding)	|
|   **w-***	|   Ancho en **%** de *1 a 100*	|
|   **col-lg-12**	|   *12* columnas de ancho max de *992px*	|
|   **justify-content-***	|   Alinea **horizontalmente**: **start, end, center, between, around**	|
|   **align-items-***	|   Alinea **verticalmente**: **start, end, center, between, around**	|
|   **align-self-start**	|   Alinea un *elemento* **verticalmente**: **start, end, center, between, around**	|
|   **order-**	|   Indica el orden:*1,2,3...*.Poner en todos	|
|   **offset**	|   Mete espacios en columnas. Info abajo.	|
|   **container-fluid**	|   **Expande** la caja al *100% de la pantalla*.	|
|   **border**	|   Crea un **borde**	|
|   **m-***	|   **Margin**: de **0 a 5** o **auto**.Cada numero son **4px**.	|
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
---

## Utilidades de Bootstrap.

> [Doc de BOOTSTRAP 4](https://getbootstrap.com/docs/4.0/utilities/borders/)

### Anchura y Altura

- **Anchura y Altura:**   
```html 
    <!-- Anchura 25 % -->
    <div class="caja w-25"></div>


    <!-- Altura 25 % -->
    <div class="container" style="height: 500px;">
        <div class="caja w-25 h-25">fsdsdf</div>
    </div>
```   
> Para que la **Altura** funcione hay que *meter la caja* en *otra caja* con una *altura dada*.   

### Bordes

- Se pone como una clase de BOOTSTRAP
```html
    <div class="border">fsdsdf</div>
    <!-- Color del border -->
    <div class="border border-warning">fsdsdf</div>
    <!-- border radius(ROUNDED) -->
    <div class="border border-warning rounded">fsdsdf</div>
    <!-- Border radius solo arriba -->
    <div class="border border-warning rounded-top">fsdsdf</div>
    <!-- Border radius solo abajo -->
    <div class="border border-warning rounded-bottom">fsdsdf</div>
    <!-- IGUAL CON LEFT Y RIGHT -->
    <!-- Sin border Radius -->
    <div class="border border-warning rounded-0">fsdsdf</div>

    <!-- Crea un circulo -->
    <div class="border border-warning rounded-circle">fsdsdf</div>

```   

### Flotados en Bootstrap
- *Se configura con la clase:*

```html
    <!-- Igual con Right -->
    <div class="float-left caja w-25 h-25 border border-warning rounded-0">Caja 1</div>
    <!-- Clase Clearfix en Bootstrap -->
    <div class="clearfix"></div>
    <!-- Se puede hacer flotados para viewport o puntos de corte de la resolucion de pantalla. A PARTIR DE SM ME QUITA EL FLOTADO. POR ABAJO-->
    <div class="float-left float-sm-none caja w-25 h-25 border border-success rounded-0">Caja 3</div>

```   

### Colores y fondos

- *Se usan las clases:*   

```html
    <!-- Color de fondo -->
    <div class="bg-warning">Caja 3</div>
    <!-- Color del texto -->
    <div class="text-secondary">Caja 3</div>
```
> Colores de [Bootstrap](https://getbootstrap.com/docs/4.0/utilities/colors/#color)   

```html
    <!-- Colores en Bootstrap -->
    <p><a href="#" class="text-primary">Primary link</a></p>
    <p><a href="#" class="text-secondary">Secondary link</a></p>
    <p><a href="#" class="text-success">Success link</a></p>
    <p><a href="#" class="text-danger">Danger link</a></p>
    <p><a href="#" class="text-warning">Warning link</a></p>
    <p><a href="#" class="text-info">Info link</a></p>
    <p><a href="#" class="text-light bg-dark">Light link</a></p>
    <p><a href="#" class="text-dark">Dark link</a></p>
    <p><a href="#" class="text-muted">Muted link</a></p>
    <p><a href="#" class="text-white bg-dark">White link</a></p>
```    


### Margenes y Paddings

- Para el **margin(m, mt, mb, ml, mr, mx, my)**:   

```html
    <div class="m-2 bg-primary text-secondary">Caja 1</div>
```
> **Cada numero de margin son 4 pixeles.**    

> **mx y my** son los ejes **y** y **x**.
>    *El X mete margenes a izquierda y derecha.*   
>    *El Y mete margenes a arriba y abajo.*    


- **Padding** igual que Margin.**padding p, pt, pb, pl, pr, px, py)**

> *Para utilizar valores negativos poner*: **m-n2**   

- La clase **mx-auto** centra en la pantalla. (**Lo mismo con Y - mx-auto**)   
```html
    <!-- centra en la pantalla -->
    <div class="mx-auto m-2 text-light p-5 bg-success caja ">Caja 3</div>
```

### Sombras
 
- **sm**, **lg** , **por defecto (shadow)** y *sin sombra* (**shadow-none**)
```html
    <div class="shadow-sm">Caja 3</div>
```

### Visibilidad

- *Oculta la caja* ; pero, **sigue estando**.    

```html
    <div class="invisible">Caja 3</div>
```   
> *Con visible se ve*    

### Textos

- **Clases** para *texto* de *Bootstrap*.    

|   **Clase**	|   **Funcion**	|
|---	|---	|
|   **display**	|   **Aumenta** tamaño fuente.(1 al 4).	|
|   **font-weight-bold**	|   **Grosor** de la fuente.**(light, italic, small)**	|
|   **text-center**	|   **Centra** _txt_ en la caja. (**right, left**)	|
|   **text-decoration-none**	|   **Quita** los puntos en los *enlaces*	|
|   **text-uppercase**    |   Cambia *txt* a **Mayusculas**.  (**lowercase**)   |

### Mostrar codigo

- Para poder poner **codigo fuente** en el Dom.

```html
    <code>
            https://www.google.com
    </code>

    <code>
        <pre>
            if($hola == "mundo"){
                echo "hola mundo";
            }
        </pre>
    </code>
    <kbd>
        Control+D para volver
    </kbd>
```

---
