---
Layout: post
Title: "¡Hola Mundo! en C/C++"
DateDay: 2010-7-14
Date: 2010-07-14T00:35:34+00:00
#Permalink: /wp/hola-mundo-en-cc.html
Categories: ["C/C++", "Código", "Programación", "simple"]
---

<blockquote><p>El siguiente post es un borrador que dejé abandonado hace ya algún tiempo, con la idea en mente de publicar algunos códigos y problemas que he resuelto en lo que he logrado participar de la OMI :), ésta vez mostraré un par de códigos, uno en C y otro en C++, ambos imprimen &#8220;Hola Mundo&#8221; a la pantalla</p></blockquote>
<p><a href="http://blog.mautematico.com/wp-content/uploads/2010/07/hola-mundo.jpg"><img class="alignright size-thumbnail wp-image-474" title="hola-mundo" src="http://blog.mautematico.com/wp-content/uploads/2010/07/hola-mundo-150x150.jpg" alt="" width="150" height="150" /></a><br />
La <a title="OMI" href="http://www.olimpiadadeinformatica.org.mx/" target="_blank">Olimpiada Mexicana de Informática</a> es un concurso de programación a nivel medio superior en México (aunque puedes participar desde primaria, según recuerdo). En ésta competencia hay dos sesiones de examen, una del simulador &#8220;Karel el Robot&#8221;, y otra propiamente de programación. El lenguaje con mayor aceptación parece ser C/C++.</p>
<p>De manera técnica, no tengo mucho que contarles de C/C++, lo que sí se es que con ellos (C++ es una extensión de C) puedes programar practicamente cualquier cosa, desde un simple &#8220;Hola Mundo&#8221; portable a varias plataformas, hasta un complejo sistema operativo completo!&#8230; Víctor (VicOMM) se molestará si no menciono que Cplusplus está orientado a la manipulación de objetos, aunque yo no estoy bien enterado de eso porque a penas se muy poco&#8230;</p>
<p>Bueno, basta ya, les mostraré un par de códigos para imprimir a la pantalla &#8220;Hola mundo&#8221;</p>
<p>El siguiente código, escrito en C, imprime a la pantalla el clásico mensaje &#8220;Hola mundo&#8221;, y termina su ejecución:</p>
{% codeblock %}
#include &lt;stdio.h&gt;
int main()
{
        printf(&quot;Hola mundo&quot;);
        return 0;
}
{% endcodeblock %}
<p><span id="more-434"></span>Y el siguiente código hace lo mismo, pero usando las clases y librerías de C++:</p>
{% codeblock %}
#include &lt;iostream&gt;
using namespace std;
int main()
{
    cout &lt;&lt; &quot;Hola Mundo&quot; &lt;&lt; endl;
    return 0;
}
{% endcodeblock %}
