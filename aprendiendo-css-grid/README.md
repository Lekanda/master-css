## CSS-GRID

#### Basicos de Grid

-Grid solo actua sobre un *div*, no sobre toda la pagina.

#### Configurar en el proyecto
 
 
1. Poner en el div quer se quiere hacer Grid:            
                `display: grid;`      
2. Con **grid-gap** le damos espaciado entre elementos en el alto y ancho.    
                `grid-gap: 10px;`
3. **grid-template-columns** : le indicamos caunats y que tamaño las columnas.    
    `grid-template-columns: 50% 50%;`  
    `grid-template-columns: calc(50% - 10px) calc(5- 10px);`    
    `grid-template-columns: calc(25% - 10px) 25% 225%;`
4. 