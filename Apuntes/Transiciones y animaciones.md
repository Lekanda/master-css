## Transiciones y animaciones

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


###### Transiciones

-Ejemplo de transicion
```css
#boton{
    display: block;
    padding: 20px;
    background-color: rgb(11, 163, 105);
    color: seashell;
    width: 200px;
    text-align: center;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-weight: bold;
    text-decoration: none;
    border: 1px solid rgb(29, 46, 3);

    
    /* transition: all 5s; */
    /* transition: border 5s; */
    transition: border 500ms, background 3000ms, border-radious 1000ms;
}
#boton:hover{
    border-radius: 15px;
    background-color: rgb(243, 111, 2);
    border: 5px solid rgb(241, 4, 4);
}
```


###### Animaciones
TODO animaciones
- 
