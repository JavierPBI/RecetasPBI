---
layout: post
---

# Crear un repositorio de funciones
Cuando las funciones se reutilizan en varios informes, lo más adecuado es mantenerlas en un repositorio común.

Ese repositorio se puede almacenar en C:\Users\User_Name\Documents\Power BI Desktop\Custom Connectors como "xxxx.mez"

Es decir, lo vamos a dejar en el mismo sitio que los custom connectors, pero esta vez el .mez no es un zip si no un simple fichero de texto que contiene todas las funciones.

La estructura de este fichero es:
```
section misFunciones;
shared mifuncion1 = (xxx as xxx) =>
    let
...
    in
        XXX;
shared mifuncion2 = ...
```
Es decir, cada función será "shared el_nombre_de la función = el_código_de_la_función" y siempre hay que terminarla con ";"

Los nombres de las funciones pueden tener prefijo tipo Date.EsFestivo = ...

En PQ pueden verse todas las funciones compartidas con #shared
