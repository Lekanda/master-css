## Posicionamiento   


###### POSICION ABSOLUTA

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

###### Z-INDEX

- Sí hay dos elementos uno encima del otro.
    - Marca que capa se superpone a la otra:
    1. **1**: La capa que la tiene
    2. **-1**: La otra capa que la tiene
    3. Si hay mas elementos *2, 3...etc*
```css
    z-index: 1;
```


###### POSICION FIJA(fixed)

- Aconpaña al hacer scroll.