<h1>Cifrado Afin</h1>
<p>El Cifrado Afin es un tipo de cifrado de sustitución monoalfabética que utiliza una función matemática para cifrar y descifrar mensajes. Este cifrado es una versión mejorada del cifrado de César, ya que utiliza dos valores enteros para cifrar y descifrar los mensajes.</p>
<h2>Descripción del código</h2>
<p>El código proporcionado es una implementación básica del cifrado Afin en Java. El código utiliza un arreglo de caracteres para representar el alfabeto español, y utiliza dos valores enteros para la "decimación" y el desplazamiento. Además, el código tiene una bandera booleana que indica si se va a cifrar o descifrar el mensaje.</p>
<p>Para cifrar un mensaje, el código utiliza la siguiente fórmula:</p>
<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>css</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-css">C = (<span class="hljs-selector-tag">A</span> * <span class="hljs-selector-tag">P</span> + <span class="hljs-selector-tag">B</span>) mod <span class="hljs-number">27</span>
</code></div></div></pre>
<p>Donde <code>C</code> es el mensaje cifrado, <code>A</code> es la posición de la letra en el alfabeto, <code>P</code> es la decimación, <code>B</code> es el desplazamiento y <code>mod 27</code> indica que el resultado debe ser reducido a un número entre 0 y 26. Para descifrar un mensaje, se utiliza la siguiente fórmula:</p>
<pre><div class="bg-black rounded-md mb-4"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>css</span><button class="flex ml-auto gap-2"><svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round" class="h-4 w-4" height="1em" width="1em" xmlns="http://www.w3.org/2000/svg"><path d="M16 4h2a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2V6a2 2 0 0 1 2-2h2"></path><rect x="8" y="2" width="8" height="4" rx="1" ry="1"></rect></svg>Copy code</button></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre hljs language-css">M = (<span class="hljs-selector-tag">A</span>^-<span class="hljs-number">1</span> * (C - <span class="hljs-selector-tag">B</span>)) mod <span class="hljs-number">27</span>
</code></div></div></pre>
<p>Donde <code>M</code> es el mensaje descifrado, <code>A^-1</code> es el inverso multiplicativo de <code>A</code> en módulo 27, y los demás valores tienen el mismo significado que en la fórmula anterior.</p>
<h2>Uso del código</h2>
<p>El código se puede utilizar como una clase independiente en un proyecto de Java. El código tiene un método <code>main</code> que se puede ejecutar para cifrar o descifrar un mensaje. Para cifrar un mensaje, establezca la bandera <code>opcion</code> en <code>true</code> y cambie el valor de la variable <code>cadena</code> para que contenga el mensaje que desea cifrar. Luego, ejecute el código y verá el mensaje cifrado en la salida estándar.</p>
<p>Para descifrar un mensaje, establezca la bandera <code>opcion</code> en <code>false</code> y cambie el valor de la variable <code>cadena</code> para que contenga el mensaje cifrado que desea descifrar. Luego, ejecute el código y verá el mensaje descifrado en la salida estándar.</p>
<p>Es importante tener en cuenta que este código es solo una implementación básica del cifrado Afin, y no debe utilizarse para fines de seguridad.</p>

