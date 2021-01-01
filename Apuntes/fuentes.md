### Fuentes en CSS

#### Fuentes y sus opciones

|   Comando	|   Explicacion	|
|---	|---	|
|   font-family	|   Aplica una fuente de txt o un grupo de fuentes	|
|   font-size	|   Tamaño de fuente de txt	|
|   font-weight	|   Ancho de la letra	|
|   font-style	|   Estilo de la letra(Italica, Oblicuo,normal..etc)	|
|   text-transform	|   Cambia de minus a mayus y mas	|
|   	|   	|
|   	|   	|


#### Fuentes Personalizadas 
#### Desde Google Fonts
1. Ir a [Google Fonts](https://fonts.google.com/).   
2. Elegir una fuente
3. Seleccionar con: **+Select this style**
4. Copiar codigo mcon metodo link o metodo style si lo hay.
5. En CSS poner el otro codigo para usar fuente.  

#### Descargando la fuente
1. Descargar una familia de fuentes desde google fonts(zip).
2. Guardar en una carpeta en folder proyecto.
3. Añadir en la hoja de estilos CSS:   
```css
/* Importar una fuente */
@font-face{
    font-family: MontserratFuenteCustom;
    src:url(fonts/Montserrat/Montserrat-Regular.ttf);
}
```
> Ahora se puede usar la `font-family: MontserratFuenteCustom;` en cualquier sitio.


#### Colores

```css
/* Colores del Sistema (https://www.w3schools.com/cssref/css_colors.asp) */
    h1{
        color: DeepSkyBlue;
        /* Colores Hexadecimales */
        color: #cccccc; 
        color: transparent;
        color: #000000;
        color: #eeeeee; 
        /* Colores RGB */
        color: rgb(156, 113, 151);
        /* Colores RGBA */
        color: rgba(156, 113, 151, 0.3);
    }
```