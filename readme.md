# Sección cards para desafio _Viajes Chile_

Las imagenes tienen diferentes resoluciones y proporciones (width/heigh). La mayoria de las imagenes tienen una proporcion cercana 1.5 (cards). Uno puede tratar de utilizar BS y CSS para hacer que todas las imagenes ocupen el mismo espacio vertical, pero es mas simple poder cambiarles su proporcion con crop y luego cambiarles su resolucion porque son excesivamente pesadas. Estos son pasos comunes, cambiar resolucion de imagenes cuando son muy pesadas/grandes.

Instrucciones:

- Instalar [imagemagick](https://imagemagick.org/script/download.php).
- Dentro de la carpeta de las imagenes ejecutar (esto yo lo hice solo con las imagenes de cards):

```
mogrify -crop '1.5:1^' *.jpg
mogrify -resize 1200x800 *.jpg
```

El comando superior **sobre-escribe las imagenes existentes**.

Con imagenes de igual proporción el código html es mucho mas simple y no es necesario agregar ningún css (solo clases BS5)
