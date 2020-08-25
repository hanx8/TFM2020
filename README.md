# INTRODUCCIÓN

<div style="text-align: justify">
El Trabajo de Fin de Master (TFM) de la Universidad Rey Juan Carlos a desarrollar tiene como tema: “Diseño y desarrollo de herramientas que automaticen la explotación de vulnerabilidades”. Él cual se ha trabajado con una aplicación Web vulnerable alojado en un Windows XP x86; diseñando, analizando y desarrollando el script de explotación en Python para explotar la vulnerabilidad de forma remota mediante Stack Buffer Overflow. La lógica y parámetros del código en Python se transformó a módulo de Metasploit, dónde se automatizó para utilizarlo de manera intuitiva.
Luego se realizó una explotación muy parecida en vez de Http con FTP, siguiendo los mismos pasos y obteniendo los mismos resultados en la explotación manual -automatizada. Con ello se creó un framework, siendo una guía para personas que deseen desarrollar sus propios módulos en Metasploit.
</div>

# DESCRIPCIÓN Y CONTEXTO

El desbordamiento de búfer es una de las vulnerabilidades más comunes en diversas aplicaciones y componentes del sistema. Una explotación exitosa de desbordamiento de búfer puede permitir la ejecución remota de código arbitrario que conduce a privilegios elevados.
Una condición de desbordamiento de búfer ocurre cuando un programa intenta insertar más datos en un búfer de los que puede acomodar, o cuando un programa intenta insertar datos en un área de memoria más allá de un búfer. En este caso, un búfer no es más que una sección secuencial de memoria asignada para contener cualquier cosa, desde una cadena de caracteres hasta una matriz de enteros. Intentar escribir fuera de los límites de un bloque de la memoria asignada puede causar corrupción de datos, bloquear el programa o incluso provocar la ejecución de código malicioso.
El Trabajo de Fin de Master (TFM) a desarrollar tiene como tema: “Diseño y desarrollo de herramientas que automaticen la explotación de vulnerabilidades”, el cual se realizará el diseño explicativo para luego realizar el análisis y desarrollo; y un framework como guía para el desarrollo de nuevos módulos.
Se realizará, la explotación de una aplicación Web vulnerable alojado en un Windows XP x86; diseñando, analizando y desarrollando el script de explotación en Python para explotar la vulnerabilidad de forma remota mediante Stack Buffer Overflow. Luego de ello la lógica y parámetros del código en Python se transformará a módulo de Metasploit, dónde se automatizará para utilizarlo de manera intuitiva.

Se muestra el escenario y la descripción:

![alt text](https://github.com/hanx8/TFM2020/blob/master/GR%C3%81FICOS/escenario.jpg)

