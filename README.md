# Examen-lenguaje-RA2

## 1A. Pregunta

En el .site-header el atributo align-items: center, choca con el justify-content: space-between. Lo que está pasando es que align-items alinea al centro solo si queda espacio libre, al usar space-between no queda espacio libre para poder centrarlo.

## 1B. Solucion

**Flexbox**

```css
.site-header {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
    
h1 {
  text-align: center;
}
```

  **Grid**

  

## 1C. Convertir cabecera

```css
.site-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
}
  
h1 {
  text-align: center;
  margin-bottom: 30px;
}
```

## 1D. Estilo del header

    .site-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-direction: column;
      /*Le añado las siguientes reglas*/
      background-color: antiquewhite; /*Fondo*/
      padding: 20px; /*Espaciado interior*/
      border-bottom: 3px solid black; /*Separacion visual*/
    }
    
    h1 {
      text-align: center;
      margin-bottom: 30px;
    }

## 2A. Boton en el header

    <header class="site-header">
        <button class="open-menu" aria-label="Abrir menú lateral">☰</button>

        <h1>Mi Sitio Web</h1>

        <nav class="main-nav">
            <li>Menu</li>
        </nav>
    </header>

## 2B. CSS nuevo

    .site-header {
      display: flex;
      justify-content: space-around;
      align-items: center;
      background-color: antiquewhite;
      padding: 20px;
      border-bottom: 3px solid black;
    }
        
    h1 {
      text-align: center;
      margin-bottom: 30px;
    }

## 3A. Miniaturas

No he podido crear las miniaturas en sí, pero lo he simulado manipulando el width de las imagenes.

## 3B. Efecto hover

Yo ya tenia esto realizado en mi página. Lo hice porque me parecía guay el efecto del zoom. Investigando diferentes transiciones encontre esta línea de código y la apliqué a mi proyecto.

## 3C. Enlace a imagen

**HTML corregido**

He añadido las etiquetas *<a>* con el enlace a la imagen original para que al pinchar te lleve a la imagen en grande. El atributo *target:"_blank"* hace que se abra en otra pestaña.

    <section id="galeria">
      <h2>Galería de imágenes</h2>
        <div class="galeria-grid">
          <a href="img/img-1.jpeg" target="_blank"><img src="img-mini/img-1.jpeg" alt="MindHunter"></a>
          <a href="img/img-2.jpeg" target="_blank"><img src="img-mini/img-2.jpeg" alt="Hombre de paco"></a>
          <a href="img/img-3.jpeg" target="_blank"><img src="img-mini/img-3.jpeg" alt="Peaky Blinders"></a>
          <a href="img/img-4.jpeg" target="_blank"><img src="img-mini/img-4.jpeg" alt="Hawaii 5-0"></a>
          <a href="img/img-5.jpeg" target="_blank"><img src="img-mini/img-5.jpeg" alt="Grimm"></a>
          <a href="img/img-6.jpeg" target="_blank"><img src="img-mini/img-6.jpeg" alt="Reina Roja"></a>
          <a href="img/img-7.jpeg" target="_blank"><img src="img-mini/img-7.jpeg" alt="Strangers Things"></a>
          <a href="img/img-8.jpeg" target="_blank"><img src="img-mini/img-8.jpeg" alt="The Witcher"></a>
          <a href="img/img-9.jpeg" target="_blank"><img src="img-mini/img-9.jpeg" alt="Alerta Cobra"></a>
        </div>
    </section>

**CSS zoom + sombra**

    .galeria-grid img:hover {
        transform: scale(1.05);
        box-shadow: 0 4px 15px rgba(0,0,0,1);
    }

## 4. Informe de evidencias

