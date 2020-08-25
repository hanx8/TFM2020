# INTRODUCCIÓN


El Trabajo de Fin de Master (TFM) de la Universidad Rey Juan Carlos a desarrollar tiene como tema: “Diseño y desarrollo de herramientas que automaticen la explotación de vulnerabilidades”. Él cual se ha trabajado con una aplicación Web vulnerable alojado en un Windows XP x86; diseñando, analizando y desarrollando el script de explotación en Python para explotar la vulnerabilidad de forma remota mediante Stack Buffer Overflow. La lógica y parámetros del código en Python se transformó a módulo de Metasploit, dónde se automatizó para utilizarlo de manera intuitiva.
Luego se realizó una explotación muy parecida en vez de Http con FTP, siguiendo los mismos pasos y obteniendo los mismos resultados en la explotación manual -automatizada. Con ello se creó un framework, siendo una guía para personas que deseen desarrollar sus propios módulos en Metasploit.

# DESCRIPCIÓN Y CONTEXTO

El desbordamiento de búfer es una de las vulnerabilidades más comunes en diversas aplicaciones y componentes del sistema. Una explotación exitosa de desbordamiento de búfer puede permitir la ejecución remota de código arbitrario que conduce a privilegios elevados.
Una condición de desbordamiento de búfer ocurre cuando un programa intenta insertar más datos en un búfer de los que puede acomodar, o cuando un programa intenta insertar datos en un área de memoria más allá de un búfer. En este caso, un búfer no es más que una sección secuencial de memoria asignada para contener cualquier cosa, desde una cadena de caracteres hasta una matriz de enteros. Intentar escribir fuera de los límites de un bloque de la memoria asignada puede causar corrupción de datos, bloquear el programa o incluso provocar la ejecución de código malicioso.
El Trabajo de Fin de Master (TFM) a desarrollar tiene como tema: “Diseño y desarrollo de herramientas que automaticen la explotación de vulnerabilidades”, el cual se realizará el diseño explicativo para luego realizar el análisis y desarrollo; y un framework como guía para el desarrollo de nuevos módulos.
Se realizará, la explotación de una aplicación Web vulnerable alojado en un Windows XP x86; diseñando, analizando y desarrollando el script de explotación en Python para explotar la vulnerabilidad de forma remota mediante Stack Buffer Overflow. Luego de ello la lógica y parámetros del código en Python se transformará a módulo de Metasploit, dónde se automatizará para utilizarlo de manera intuitiva.

Se muestra el escenario y la descripción:

![alt text](https://github.com/hanx8/TFM2020/blob/master/GR%C3%81FICOS/escenario.jpg)

# DESARROLLO DEL CÓDIGO MANUAL Y EL MÓDULO AUTOMATIZADO(HTTP)

Parte del procedimiento del desarrollo del código/módulo automatizado, se tiene que realizar el reconocimiento dónde encontraremos IP, Puerto, versión de sistema operativo y de la aplicación vulnerable para insertarlo al script; luego en el análisis se interceptará el tráfico HTTP en este caso validando los parámetros utilizados.
Conforme se va desarrollando el código, vamos analizando con Immunity Debugger, calculamos el offset y bad caracter para seguir con la explotación. Al ejecutar el código manual/módulo automatizado, explotaremos la vulnerabilidad de stack buffer overflow dentro de Windows XP SP3 en la aplicación vulnerable (Integard versión 2.2); al ser explotada la máquina víctima enviará un Reverse TCP y le dará acceso al atacante mediante Meterpreter.
El detalle de lo mencionado se encuentra en:

https://github.com/hanx8/TFM2020/blob/master/TFM%202020-Hans%20L%C3%B3pez%20Mendoza.pdf

Código manual:

https://github.com/hanx8/TFM2020/blob/master/SCRIPT%20MOD%20HTTP/exploit_integard.py

Módulo automatizado en Metasploit:

https://github.com/hanx8/TFM2020/blob/master/SCRIPT%20MOD%20HTTP/mod_exploit.rb

# DESARROLLO DE OTRO MÓDULO EXPLOTANDO OTRA VULNERABILIDAD MUY SIMILAR(FTP).

Se explotó otra vulnerabilidad muy parecida en vez del servicio HTTP en este caso es con FTP. Tipo de explotación remote stack buffer overflow en Windows XP SP3 x86. Siguiendo los mismos pasos demostrados con la vulnerabilidad anterior. Este Item, está basado en el objetivo

El detalle de lo mencionado se encuentra en:

https://github.com/hanx8/TFM2020/blob/master/TFM%202020-Hans%20L%C3%B3pez%20Mendoza.pdf

Código manual:

Módulo automatizado en Metasploit:


























