# CSS-GRID

### Basicos de Grid

- *Grid* solo actua sobre un *div*, no sobre toda la pagina.   
- *Grid* acepta mejor las **fracciones(fr)**. Mejor que **%**.
---
### Configurar y manejar GRID en el proyecto.
 
1. Poner en el div quer se quiere hacer Grid:            
                `display: grid;`      
2. Con **grid-gap** le damos espaciado entre elementos en el alto y ancho.    
                `grid-gap: 10px;`
3. **grid-template-columns** : le indicamos cuantas y de que tamaño son las columnas.    
    `grid-template-columns: 50% 50%;`   

    `grid-template-columns: calc(50% - 10px) calc(5- 10px);`    

    `grid-template-columns: calc(25% - 10px) 25% 25%;`       

    `grid-template-columns: repeat(4,calc(25% - 10px));`       

    `grid-template-columns: repeat(2,calc(25% - 10px)) 15% 35%;` 

    ```css
    /*fr => Fraccion. Le indicamos la fraccion de el div que ocupa.
     1fr => 1 columna
     2fr => 2 columnas
     */
    grid-template-columns: 1fr 1fr;
    grid-template-columns: repeat(4, 1fr);           
    ```         
4. **grid-template-rows**: Le indicamos numero de filas.         
    `grid-template-rows: 1fr 1fr 1fr;`         
    `grid-template-rows: 50% 10% 35%;`     
    `grid-template-rows: 1fr 2fr 1fr;`   
    `grid-template-rows: repeat(2, 1fr) 3fr;`    

5. Para expandir las columnas se usa **grid-column-start** y **grid-column-end**.
    - El *layout* esta definido en el punto *3* y *4*.   
    ```css
    /*Con el Start le decimos desde donde y con el end hasta donde*/
        grid-column-start: 1; 
        grid-column-end: 3;
    /*Esto se puede hacer en una linea con*/
        grid-column: 1 / 3;
    ```  
    
> Lo mismo con  **grid-row**
---

### Centrar contenido en una caja   

- Convertir la caja a *Flex*.   
```css
#cabecera{
    display: flex;
    justify-content: center;
    align-items: center;
}
```   


### GRID-AREA y Areas en grid.

- Es otra forma de maquetar los *divs*.

```css
/* De esta forma creamos la plantilla en el div general. */
#website-area{
    grid-template-areas: 
        "cabecera cabecera cabecera cabecera cabecera"
        "lateral menu menu menu menu"
        "lateral contenido contenido contenido contenido"
        "lateral pie pie pie pie"
        ;

}
/* De esta forma  ligamos el elmento con la plantilla de arriba*/
#website-area #cabecera{
    grid-area: cabecera;
}
#website-area #menu{
    grid-area: menu;
}
```

- 