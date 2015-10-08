---
layout: post
title: 'JavaScript: string startsWith()'
date: '2015-10-07'
---

If you ever need to know in your JavaScript application if a _string_ starts with another _string_, you can just use new _ECMAScript 6_'s method: `startsWith()`

<code><var>str</var>.startsWith(<var>searchString</var>[, <var>position</var>])</code> will take
- as first parameter: <var>searchString</var>, the characters you want to know are or not at the beginning of <var>str</var>
- as optional parameter: <var>position</var> the index you want the search to start.

<h2 id="Examples">Examples</h2>
<h3 id="Using_startsWith()">Using <code>startsWith()</code></h3>

<pre class="brush: js">
var str = 'To be, or not to be, that is the question.';

console.log(str.startsWith('To be'));         // true
console.log(str.startsWith('not to be'));     // false
console.log(str.startsWith('not to be', 10)); // true
</pre>

<h2 id="Polyfill">Polyfill</h2>

Please keep in mind: old browsers do not implement `startsWith()`. Here you have a _Polyfill_ for those old browsers:

<pre class="brush: js">
if (!String.prototype.startsWith) {
&nbsp; String.prototype.startsWith = function(searchString, position) {
&nbsp;&nbsp;&nbsp; position = position || 0;
&nbsp;&nbsp;&nbsp; return this.indexOf(searchString, position) === position;
&nbsp; };
}
</pre>

<h2 id="See_Also">See also</h2>

Please refer to MDN if you have any further questions on this. <br /> [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/startsWith#Syntax](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/startsWith#Syntax)

There you will get not only up-to-date documentation for `startsWith()`, but also references to related methods and a more robust Polyfill.
