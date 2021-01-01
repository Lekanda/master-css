#### Fondos

##### background   
- Se le puede poner un color directamente.
- **background: red imagen repeticion posicion**
- Aunque funciona , es mejor para el color de fondo utilizar **background-color**. Es menos lioso

##### background-image     
- Forma normal de ponerlo        
```css
    background-image: url(img/patron2.png);
```  
##### background-repeat    
- Forma normal de ponerlo       
```css
    background-repeat: repeat;

```  
###### Opciones del background-repeat
> 1. repeat = repite la imagen
> 2. repeat-x = repite la imagen solo en el eje X
> 3. repeat-y = repite la imagen solo en el eje Y
> 3. no-repeat = no repite la imagen


##### background-size    
- Forma de uso.             
```css
    background-size: 15px;

```  
###### Opciones del background-size
> 1. %
> 2. px



##### background-attachment: fixed;   
- Forma de uso.             
```css
    background-attachment: fixed;

```  
###### Opciones del background-attachment
> 1. fixed = La imagen de fondo no se mueve



##### background-position  
- Forma de uso.             
```css
    background-position: right;

```  
###### Opciones del background-position  
> 1. center = La imagen de fondo se centra
> 2. igual con left, right,top y bottom



background-position: center;