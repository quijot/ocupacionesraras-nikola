<link rel="stylesheet" href="/assets/css/font-awesome.css">
<!-- 
.. description: 
.. link: 
.. tags: Nikola,Wordpress
.. slug: mudanza-hacia-nikola
.. title: Mudanza hacia Nikola
.. date: 2013/05/28 14:43:23
-->

Mi anterior blog estaba hecho en [Wordpress][wp]. Hago un breve raccontto de su mutación.

- v1.0: Estuvo alojada en http://ocupacionesraras.wordpress.com (y sigue estando ahí).
- v2.0: Me reservé el dominio **ocupacionesraras.com.ar** en el **nic.ar** y lo alojé en **000webhost.com** (hosting gratarola). Seguía siendo Wordpress.
- v3.0: Es el momento de [Nikola][nikola], el static blog generator hecho por [Roberto Alsina](http://ralsina.com.ar/). Sigue alojado en 000webhost.com. Ahora tengo el código en un repositorio público de github.

### Cómo hice

Exporté el contenido del blog desde wordpress con la herramienta de exportación propia del wordpress. Genera un archivo xml con el contenido (en este caso el nombre del archivo ``or-mayo.xml``). Sencillísimo. Luego, ya instalado el Nikola, etc., usé el comando de importación automática de Nikola:

    #!bash
    $ nikola import_wordpress -o ocupacionesraras-nikola or-mayo.xml

y casi listo. Sólo tuve que retocar a mano algunas cositas.

### Azuquitar

El blog figura en la [lista oficial](http://nikola.ralsina.com.ar/some-sites-using-nikola.html) de sitios hechos con Nikola.

Nikola soporta temas. Estoy usando el tema **cortazar**, basado en el [theme](https://github.com/mgaitan/my-nikola-theme) hecho por [Martín Gaitán](mgaitan.github.com).

Sitio y tema tienen sus repositorios de [github][gh]:

<ul style="list-style-type: none;">
    <li><i class="icon-github"></i> blog: <a href="https://github.com/quijot/ocupacionesraras-nikola">ocupacionesraras-nikola</a></li>
    <li><i class="icon-github"></i> theme: <a href="https://github.com/quijot/cortazar-theme">cortazar-theme</a></li>
</ul>

[wp]: http://wordpres.com
[nikola]: http://nikola.ralsina.com.ar
[gh]: http://github.com
