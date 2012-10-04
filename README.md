Tema: Editor de fórmulas matemáticas
======
**Direccion gist: prueba de la librería**

gist.github.com/3831478

**Investigar sobre el tipo de contenido asignado.**

Los editores de fórmulas matemáticas son herramientas creadas para traducir el lenguaje matemático (fórmulas, resultados) a expresiones digitales que se puedan manipular más fácilmente. Las más comunes están en línea; los que usan WYSIWYG (permite escribir un documento viendo directamente el resultado final) dan la opción de barras de herramientas para un manejo más sencillo, si no se usarían un lenguaje de interpretación que requiere de cierto nivel de conocimiento por parte del usuario.
 
**Elementos y propiedades principales.**

Entre los principales elementos de un editor de fórmulas matemáticas están:
Crear, presentar y editar ecuaciones. El editor debe ser capaz de abrir archivos .xml con el contenido de la fórmula matemática a mostrar o editar.
 
**Forma de visualización**

La idea es mostrar las fórmulas matemáticas que entran en formato de marcas XML como una ecuación matemática, así un archivo con un contenido como este:
 
     <math>
     <apply>
    	     <plus/>
    	     <apply>
        	<times/>
        	<ci>a</ci>
        	<apply>
            	<power/>
            	<ci>x</ci>
            	<cn>2</cn>
        	</apply>
    	</apply>
    	<apply>
        	<times/>
        	<ci>b</ci>
        	<ci>x</ci>
    	</apply>
    	<ci>c</ci>
      </apply>
      </math>
 
Presentaría la ecuación siguiente:

[logo]: http://upload.wikimedia.org/math/5/b/7/5b7bc9adb96a6ee1dc17b024f1ddab74.png
[google]: http://www.google.com/ "clic para visitar Google.com"
[![logo de google][logo]][google]


 
**Librerías consultadas**

**MathML**

“El MathML o Mathematical Markup Language es un lenguaje de marcado basado en XML, cuyo objetivo es expresar notación matemática de forma que distintas máquinas puedan entenderla, para su uso en combinación con XHTML en páginas web, y para intercambio de información entre programas de tipo matemático en general”.
 
**1. MathML.js**

Es una aplicación de XML para describir notaciones matemáticas y la captura de su estructura y contenido.
                                                (X+Y)2

      <math>
      <msup>
      <mrow>
     	<mo> ( </mo>
      <mrow>
      <mi> x </mi>
      <mo> + </mo>
      <mi> y </mi>
       </mrow>
     <mo> ) </mo>
      </mrow>
      <mn> 2 </mn>
     </msup>
      </math>


**2.LatexMath.js y AsciiMath.js**

LatexMath es una modificación de AsciiMathML.js, por Peter Jipsen. Y modifica poco la sintaxis a la hora de la implementación.

           Ejemplo LatexMath:
           <blockquote>$\begin{eqnarray} x & = & \frac{-7 \pm \sqrt{49 - 24}}{6} \\
           & = & -2 \textrm{ or } -\frac13. \end{eqnarray}$</blockquote>
        	Resultado:
        	           	x=-7±49-246=-⅓ or -2

          Ejemplo AsciiMath:
                        `sum_(i=1)^n i=(n(n+1))/2`
          Resultado:
                       ∑i=1ni=n(n+1)2 

**3. Mathjax.js**

 Es una librería tipo OpenSource que incluye un motor de visualización para Javascript, y que funciona en todos los browsers modernos. Sus principales características son:
* Tipografía de Alta Calidad. MathJax utiliza CSS y fuentes web modernas, en lugar de imágenes de ecuación o Flash, por lo que las ecuaciones a escala son de excelente calidad a todos los niveles de zoom.
* Es permitido en todos los browsers modernos, por lo que los cálculos en tu sitio pueden ser vistos claramente por prácticamente todos los lectores, incluso los que utilizan los teléfonos inteligentes.
* Es de fácil integración en web pages, blogs, y otras aplicaciones web.
* Permite a los lectores copiar las ecuaciones matemáticas que generaron y pegarlas donde así lo deseen.
* Permite a los desarrolladores crear materiales interactivos de cursos, herramientas avanzadas de creación, y aplicaciones que permitan ecuaciones matemáticas.
* Es compatible con los lectores de pantalla utilizados por personas con discapacidad visual, y la función de zoom permite a todos los lectores ver pequeños detalles de las ecuaciones.
 
**Bibliografía**

 MathML - Wikipedia, la enciclopedia libre (s. f.). Recuperado de http://es.wikipedia.org/wiki/MathML
 
LaTeXMathML: a dynamic LaTeX mathematics to MathML converter (s. f.). Recuperado de http://www.maths.nottingham.ac.uk/personal/drw/lm.html

 LaTeXMathML.js (s. f.). Recuperado de http://www.maths.nott.ac.uk/personal/drw/LaTeXMathML.js
 
 ASCIIMathML.js (s. f.). Recuperado de http://www1.chapman.edu/~jipsen/mathml/ASCIIMathML.js
 
http://www.mathjax.org/

 
