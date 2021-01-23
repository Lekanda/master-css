# Master en CSS por Victor Robles

> *Fecha Inicio 18-12-2020*

### Selectores
|   Forma	|   Sintaxis	|
|---	|---	|
|   Etiqueta	|   Nada	|
|   Clase	|   .	|
|   Id	|   #	|


- Se puede compartir una clase con varias: etiquetas,....etc
```css
    #descripcion,
    #titulo{
    border: 2px solid black;
    padding:15px;
}
```   

###### Pointers del Raton
![Pointers](Apuntes/ImagenesApoyo/PointersEnCSS.jpg)      
> Tipos de Pointers


###### Estructura de un BACKGROUND
`background: red imagen repeticion posicion`


> `margin: 0px auto;` => Centra el bloque


###### border-radius   

- general
```css
    border-radius: 5px ;
```
- Las cuatro esquinas
```css
    border-radius: 5px 5px 5px 5px;
```

###### overflow

- Cuando los elementos de una caja son mas grandes que la caja. Hay opciones:
    1. **hidden**: Borra lo que no entra.
    2. **visible**: Es visible.
    3. **scroll**: Hace scroll.
    4. 

> Para quitar la barra de scroll horizontal:
        ```css
        overflow-y:scroll
        ```

###### Posicion absoluta y fija

- Se puede posicionar completamente.
- Mediante **px** o **%**
```css
    .libre{
        position: absolute;
        top: 250px;
        left: 10%;
        border: 1px solid black;
        background-color: red;
        color: white;
        width: 50px;
        height: 50px;
        font-size: 13px;
    }

```
> La *fija* igual pero en `position: fixed;`



###### Pseudoclases

|   Pseudoclase	|   Explicacion	|
|---	|---	|
|   **li:first-child**	|   Coge el primer **li**.	|
|   **li:nth-child(3)**	|   Coge el **3º**.	|
|   **li:last-child**	|   Coge el ultimo **li**.	|
|   **#mi-enlace:link**	|   link visitado PR.E	|
|   **#mi-enlace:visited**	|   Link visitado PERSO.	|
|   **#mi-enlace:hover**	|   Cuando pasa raton por encima.	|
|   **#mi-enlace:active**	|   Cuando presionas con el raton.	|
|   **input[type="text"]:focus**	|   Esta el foco en el(Formularios)	|
|   	|   	|












```css
$grid-breakpoints: (
  xs: 0,
  sm: 576px,
  md: 768px,
  lg: 992px,
  xl: 1200px,
  xxl: 1400px
);
```
- Enlace a Wiki
- Enlace a GitHub-Pages