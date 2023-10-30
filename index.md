---
title: "Sintaxis Básica Markdown"
author: "Renzo Cáceres Rossi"
date: "30-10-23"
subtitle: "Markdown - RMarkdown"
output:
  html_document:
    toc: TRUE
    toc_float: TRUE
    code_download: TRUE
---

<!-- Crear documentos reproducibles en RStudio usando Markdown -->

## Sintaxis Markdown

**Markdown** es un lenguaje de marcado ligero (***Lightweight Markup Language***),siendo **RMarkdown**[^pie_pagina_01], uno de sus dialectos, una de sus varianetes, uno de sus sabores (**Markdown Flavours**)


## Encabezados - Títulos 

```
# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6

Título 1
=========

Título 2
---------

```

## Separaciones - Líneas Horizontales

---

---

***

***

## Citas - Añadir citas a nuestro documento Markdown

> "La gente que está lo suficientemente loca para pensar que que pueden cambiar el mundo es la gente que lo consigue"
>
> **Steve Jobs**


## Formateado de texto - Negrita - Cursiva - Tachado - Subrayado

**Texto formateado como Negrita**

*Texto formateado como Cursiva*

***Texto formateado como Negrita y Cursiva***

~~Texto tachado~~

<u>Texto Subrayado</u> <!--HTML Tags-->


## Listas

### Lista Anidada - Lista Viñetas

- Lista 1
- Lista 2
- Lista 3
- Lista 4
- Lista 5
  - Lista 5.1
  - Lista 5.2
  - Lista 5.3
- Lista 6
- Lista 7
- Lista 8

### Lista Numerada

1. Lista 1
2. Lista 2
3. Lista 3
4. Lista 4
5. Lista 5
6. Lista 6
7. Lista 7

### Lista ordenada alfabéticamente

a. Lista A
b. Lista B
c. Lista C
d. Lista D
e. Lista E
f. Lista F

### Casos - Ejemplos

- Lista 1
- Lista 2
- Lista 3
+ Lista 4
+ Lista 5
+ Lista 6
* Lista 7
* Lista 8
* Lista 9

1. Lista 1
3. Lista 2
5. Lista 3
7. Lista 4
9. Lista 5
11. Lista 6
13. Lista 7

## Tablas - Añadir tablas a nuestro documento Markdown

|TABLA A|TABLA B|TABLA C|
|:-----:|:-----:|:-----:|
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |


## Enlaces - Añadir links a nuestro documento Markdown

<https://www.youtube.com/c/RenzoCaceresRossi>

[Renzo's Youtube Channel](https://www.youtube.com/c/RenzoCaceresRossi){target=_blank}

[Suscribete a mi canal de YouTube](https://www.youtube.com/c/RenzoCaceresRossi "Click Suscribete")



## Imágenes - Añadir imágenes a nuestro documento Markdown

<center>

![](diagrama_barras_amano.jpg){width=400 height=300}

</center>


<center>


![](https://d33wubrfki0l68.cloudfront.net/aee91187a9c6811a802ddc524c3271302893a149/a7003/images/bandthree2.png){width=500 height=400}

</center>

## Vídeos - Añadir vídeos de YouTube a nuestro documento Markdown

<center>

<iframe width="560" height="315" src="https://www.youtube.com/embed/5k_1fNIScuU?si=hhOmmgkRjYuve-fX" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen data-external=1></iframe>

</center>


## Mapas - Añadir mapas (Google Maps) a nuestro documento Markdown

<center>

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3901.964602015342!2d-77.0331073257089!3d-12.045956541884093!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c8b5d5aa7eb1%3A0x16061e0b481e22aa!2sPlaza%20Mayor%20de%20Lima!5e0!3m2!1ses-419!2spe!4v1698679673938!5m2!1ses-419!2spe" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade" data-external=1></iframe>

</center>


## Código - Añadir código de distintos lenguajes de programación (R-Python-SQL)

    summary(mtcars)
      
La función base `barplot()` nos permite crear diagramas de barras (**Bar Charts**) en el lenguaje de programación R.

~~~
x <- table(mtcars$cyl)

colores <- c("orange","blue","purple")

barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)
~~~

```R
x <- table(mtcars$cyl)

colores <- c("orange","blue","purple")

barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)

```

```Python
import matplotlib.pyplot as plt
 

eje_x = ['Python', 'R', 'Node.js', 'PHP']
 

eje_y = [50,20,35,47]
 

plt.bar(eje_x, eje_y)
 

plt.ylabel('Cantidad de usuarios')
 

plt.xlabel('Lenguajes de programación')
 

plt.title('Usuarios de lenguajes de programación')
 

plt.show()

```

```SQL
USE Northwind;

SELECT * FROM Products;
```

## Anular sintaxis Markdown


\ # Esto debería ser un Título tipo 1


\**Esto debería ser texto formateado como Negrita**


\*Esto debería ser texto formateado como Cursiva*

[^pie_pagina_01]:**RMarkdown es un paquete (package) del lenguaje de programación R que nos permite crear documentos reproducibles en formatos tales como HTML,PDF,Microsoft Word entre otros.**


<div class="tocify-extend-page" data-unique="tocify-extend-page" style="height: 0;"></div>

