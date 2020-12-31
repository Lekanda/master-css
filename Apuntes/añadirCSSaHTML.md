##### Formas de conectar un HTML a CSS

1. En la etiqueta HTML.
    ```html
        <h1 style="background: rgb(228, 183, 183); color: red;">Master en CSS</h1>  
    ```  

2. Añadirlo en el HEAD del HTML
```html 
    <style type="text/css">
        h1{
            color: rgb(90, 53, 5);
            font-size: 50px;
            text-shadow:0px 0px 10px cornflowerblue;
            text-decoration: underline;
        }
    </style>
```   

3. **ESTA ES LA CORRECTA!!**. Mediante un link a un archivo CSS.   
    
```html
    <link rel="stylesheet" type="text/css" href="styles.css">
```  
> En este caso el archivo **styles.css** esta en la misma carpeta.