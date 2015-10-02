---
Layout: post
Title: "Código para sumar dos números"
DateDay: 2010-11-3
Date: 2010-11-03T00:18:02+00:00
#Permalink: /wp/codigo-para-sumar-dos-numeros.html
Categories: ["C", "C/C++", "compilar", "enteros", "Mates", "ocio", "programa", "Programación", "sencillo", "simple", "sumar", "variables"]
---

<blockquote><p>Dos posts seguidos sobre el mismo tema? :S&#8230; creo que le han absorbido las ideas a mi cabeza!&#8230; </p></blockquote>
<p>Hoy, pretendiendo que éste sea un post simple, voy a presentarles un código simple: uno en C++ que suma dos números dados por el usuario (a y b). AH!.. números enteros:</p>
<pre class="brush: cpp; title: ;">
#include &lt;iostream&gt;	//Libreria requerida para usar cin y cout
using namespace std;	//instruccion para el uso de cin y cout
int a,b;		//definimos dos variables de tipo int (integer=entero)
int main()		//Aquí va la función principal de nuestro programa
{
cin&gt;&gt;a&gt;&gt;b;		//Leemos del teclado los enteros a y b
cout&lt;&lt;endl&lt;&lt;a+b&lt;&lt;endl;	//imprimimos un salto de linea (endl), la suma de a+b y luego otro salto de línea
//	Descomentar para usar como ejecutable en windows
//    system(&quot;Title Programita que suma dos numeros&quot;);
//    system(&quot;PAUSE&quot;);
    return 0;
}
</pre>
<p>Por si se lo preguntan, hay que compilarlo.<br />
Pueden compilarlo desde terminal/consola, pero en caso que estén en:<br />
Linux o MacOS: Pueden usar algo como <a href="http://www.codeblocks.org">CodeBlocks</a><br />
Windows: <a href="http://www.codeblocks.org">CodeBlocks</a> o <a href="http://www.bloodshed.net/dev/devcpp.html">Dev-C++</a><br />
BSD y demás: JA!&#8230; como si tuviera lectores usuarios de BSD que no tuvieran maneras chidas de compilar <img src=&#39;http://blog.mautematico.com/wp-content/plugins/smilies-themer/kopete/smile.png&#39; alt=&#39;:)&#39; class=&#39;wp-smiley&#39; /> </p>
<p>Puede que se me pasaran algunas cosas, para eso están los comentarios :). Obviamente acepto sugerencias!<br />
Nota al margen: estoy pensando a que destinar <a href="http://www.geeksoy.com/">www.geeksoy.com </a></p>
