---
layout: post
Title: "“¡Hola, mundo!” en JavaScript, en la consola de Firefox"
dateDay: 2015-1-4
date: 2015-01-04T07:07:43+00:00
#Permalink: /wp/hola-mundo-en-javascript-en-la-consola-de-firefox.html
categories: ["Sin Categoria"]
---

<p>En el trozo de espacio-tiempo en que me encuentro al escribir esto, los pasos que intentaré describir a continuación suelen dar <em>vida</em> a pequeños monstruos, en sí mismos inofensivos, pero no por eso triviales. De hecho, cuentan las leyendas que monstruos temibles, atroces, feroces y hasta molestos han sido resultado de un proceso natural de evolución y mutaciones de pequeños y tiernos monstruos, como esos a los que me referí en primer lugar.</p>
<p>Me atrevo a suponer, anónimo y estimado internauta, que mis instrucciones permanecen vigentes y válidas en tu realidad actual, en ese futuro desde el que me lees. ¡Perdóname si no es así!</p>
<p>Te advierto desde ya, que hoy (mi hoy) me atreví a ser fan del filtro de pixelado, una vez que me di cuenta que se escapa a mis capacidades actuales enviar este mensaje a los futuros sin la pérdida de, al menos, la información irrelevante en las imágenes.</p>
<p>¡Te mostraré cómo programar el mensaje <em>¡Hola, mundo!</em> (mundo futuro, supongo) en JavaScript!</p>
<p>Lo que necesitamos:</p>
<ol>
<li>Un programa donde escribir texto <span style="text-decoration: underline;">sin formato</span> (<em>a.k.a. texto plano</em>), para escribir nuestro programa.
<ul>
<li>Si colorea el código, ¡de lujo!</li>
</ul>
</li>
<li>Un motor de ejecución JavaScript (<em>a.k.a máquina virtual JavaScript</em>), para ver nuestro programa en acción.</li>
</ol>
<p>En este momento de mi vida, una de las cosas que me encantan sobre JavaScript es que es realmente portable. ¡Casi todo lo que sea una computadora está listo para ejecutar un programa escrito en JS! Porque resulta ser que casi todo lo que sea una computadora tiene instalado un navegador Web que viene con lo que pedimos en el punto 2.</p>
<p>Lo que usaremos:</p>
<p><a title="Firefox, el mejor navegador Web" href="https://affiliates.mozilla.org/link/banner/54363" target="_blank"><strong>Mozilla Firefox</strong></a>, el mejor navegador Web de nuestro sistema solar. Con varios editores de texto plano incluidos.</p>
<p>Yo usaré la versión 34 de Firefox (que es la más reciente y estable en este trozo de espacio-tiempo). Tú puedes usar la dos mil quince si así lo deseas. Con suerte.</p>
<p>Una vez que tu Firefox haya iniciado, estás listo para aprender cómo abrir la Consola Web. Tienes varias opciones, mis favoritas son las primeras dos:</p>
<ul>
<li>CTRL + Shift + K (reemplaza CTRL por CMD si usas Pera OS)</li>
<li>Shift + F12</li>
<li>Presiona Alt y luego muévete por los menús que se muestran a continuación:</li>
</ul>
<figure style="width: 681px;" class="wp-caption aligncenter"><a href="http://blog.mautematico.com/wp-content/uploads/2015/01/abrir-consola-menú.png"><img src="http://blog.mautematico.com/wp-content/uploads/2015/01/abrir-consola-menú.png" alt="" width="681" height="388" /></a><figcaption class="wp-caption-text">Figura 1: Secuencia del menú para abrir la consola: Herramientas » Desarrollador Web » Consola Web</figcaption></figure>
<p>¡Felicidades! ya completaste la mitad tediosa del camino. Ahora viene la mitad BBB (buena, breve y blue).</p>
<p>Típicamente la consola hará un espacio a la derecha (»») de la pantalla para colocarse en él. La Consola Web viene acompañada de varios amigos, a quienes espero tener el placer de presentarte en otra ocasión. Por ahora:</p>
<p>¡Consola del futuro, <em>anónimo y estimado internauta del futuro</em>, os presento!</p>
<p>Consola no es en realidad un editor de texto, pero será un excelente auxiliar para la misión que me encomendaron encomendarte. Escribe en ella el siguiente código, y al final <em>mándalo</em>, con la tecla enter/intro/return/retorno de carro:</p>
<pre class="brush: jscript; title: ; notranslate">
alert(&quot;¡Hola, mundo!&quot;);
</pre>
<p>El resultado, como te prometí, suele ser un pequeño y tierno monstruo como el que te muestro a continuación:</p>
<figure style="width: 587px;" class="wp-caption aligncenter"><img src="http://blog.mautematico.com/wp-content/uploads/2015/01/javascript-alert-consola1.png" alt="" width="587" height="334" /><figcaption class="wp-caption-text">Figura 2: Ventana emergente mostrando el texto &#8220;¡Hola, mundo!&#8221;, como se indica en la Consola Web</figcaption></figure>
<p><em>Et voilá</em>, ¡ya has programado algo &#8211;no mucho- en JavaScript!</p>
<p>Como quizás notaste, fue un programa muy simple y el monstruo creado no es, que digamos, muy molesto. Si juegas un poco con el texto en medio de las comillas podrás personalizar el mensaje y cambiarlo por un <em>¡Hola, cara de bola!</em>, y casi cualquier cosa que quieras.</p>
<hr />
<p>Bonus 1:</p>
<p>En otro pasado programaba un poquito en C/C++ y escribí un post para que puedas seguir procrastinando un rato escribiendo <a title="¡Hola, mundo! en C/C++" href="http://blog.mautematico.com/2010/hola-mundo-en-c.html" target="_blank"><em>¡Hola, mundo!</em> en C/C++</a>.</p>
<p>Te advierto que en aquel post no recomendé ningun compilador. Ahora te recomiendo CodeBlocks, que puedes descargar en un paquete junto con <em>gcc</em> y <em>g++ </em>(que son los compiladores que te recomiendo).</p>
<p>Bonus 2 (zona de riesgo):</p>
<p>Si tecleas al azar (incluyendo la tecla para borrar) infinitamente, la probabilidad de que en algún momento obtengas el siguiente código es 1 (100%):</p>
<pre class="brush: jscript; title: ; notranslate">
while(true) alert(&quot;dsda&quot;);
</pre>
<p>Código que suele dar vida a más monstruos. ¡No lo ejecutes!</p>
