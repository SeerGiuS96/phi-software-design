- # Preface
  
  La gente ha escrito programas electricos durante mas de 80 años, pero rara vez han hablado de como diseñar estos prograbas o como deberia de lucir un buen programa. Ha habido mucha discusion sobre el proceso del desarrollo de software con metodologias como agile, y herramientas como debuggers, control de version, y covertura de test. Tambien hay un extenso analisis de tecnicas de programar como orientada  a objetos, y programacion funcional, y patrones de diseño y algoritmos. Todos estas discusiones tiene valor, pero todavia hay una gran parte sin tocar. aunque en el 1971 David Parns menciono algo en "Decomposing system into modules", pero no ha progresado mas en 45 años.          El problema fundamental en la cienca de la computacion es la descomposicion: como hacer algo complejo dividirlo en piecas que se resuelvan independientemente.  Es el problema principal al que se enfrentan los programadores dia a dia, porque no se habla del diseño del software.  
  hace referencia a un libro "Talent is Overrated by Geoff Colvin)." porque hay programadores buenos que si saben diseñar software pero no saben explicarlo.  
 Entonces este autor, para buscar respuesta a todas estas preguntas decide crear un curso, se llama "CS 190" en la universidad de Standford.

 C1 Its all about complexity
 escribir software es una de las actividades mas puras en la historia del humano. Los programadores no estamos limitados por la ley de la fisica. podemos crear exitantes palabras  virtuales con comportamientos que nunca podrian existir en el mundo real. Ademas, programacion no requiere habilidad fisica o coordinacion como futbol o baloncesto. Lo que requiere es:
 una mente creative
 la habilidad de organizar tus ideas.

 La mayor limitacion de escribir software es entender lo que creamos. cuanto mas crezca, mas complicado es. Esto realentiza el desarrollo y añade costes. Cuanto mas grande, y mas gente trabaje ne el , mas dificil es de manejar.

 Hay herramientas que ayudan a manejar la complejidad. Si reducimos complejidad, podemos construir mas sistemas potentes siendo barato. Cuanto mas sencillo sea el diseño mas grande podemos construir el proyecto.

 hay 2 formas de conseguirlo, que se discutiran en este libro
 - Eliminar la coplejidad haciendo codigo simple y obvio.
 - encapsular, para que los programadores puedan seguir trabajando sin extar expuestos a la complejidad. esta tenica se llama trabajar por modulos. Estan diseñados para se relativamente independientes unos de otros, para que el programador pueda trabajar en un modulo sin tener que entender detalladamente los otros

 Cambios grandes de diseño arquitetura son un reto mas que los sistemas fisicos. un ejempo claro se ve que un puente, no puedes cambiar los soportes en medio de la construccion.

 Desarrollo incremental significa que el diseño del software nunca termina. El diseño ocurre continuamente sobre la vida de u nsistema.

 El libro tiene 2 objetivos:
 1 que significa la "complejidad" y que hace. Por que importa y como reconocer cuando un programa tiene complejidad innecesaria.
 2. tecnicas aplicables durante el desarrollo para minimalizar complejidar. Desafortunadamente no hay una receta simple que garantize un buen diseño de sistema.

 ## 1.1 how to use this book 
Muchos de los diseños descritos aqui son abstractos, asi que sera dificil apreciarlos sin ver codigo. Le ha sido dificil al autor encontrar ejemplos que sean lo suficientemente pequeños para incluirlos en el libro.

La mejor forma de usar este libro es cojutnamente con revisiones de codigo. cuando revisas el codigo de otra persona, es mas facil de ver los problemas de diseño mas que en tu propio codigo.

Para mejorar, el va a usar las red flags. si ves una, intenta refactorizarla buscando diseños alternativas antes de dar co nla que soluciona el problema. No te rindas facilmente, cuantos mas hagas, mas aprenderas.

Cuando apliques alguna idea de este libro, es importante que te moderes y sean discretos. Cada regla tiene excepciones, y cada principio tiene sus limites. Si te pasas y lo llevas a un extremo probablemente acabe mal. Los diseños bonitos reflejan balance entre competing ideas y approaches. En muchas capitulos el autor ha puesto secciones "taking it too far" indicando cuando se "overdoing" una buena cosa.

Todos los ejemplos estan en java o C++, y orientado a objetos. pero tambien estas ideas se pueden aplicar a lenguajes que no son orientado a objetos como C.

# Chapter 2
En este libro, complejidad se define de una forma practica: Es cualquier cosa relacionada con la estructura del sistema de software que hace dificil entender y modificar el sistema.

Se puede apareceder de muchas formas. por ejemplo, puede ser dificil entender un trozo de codigo.

Los proyectos grandes suelen tener complejidades complejas por lo general si no se a pensado e nel diseño, pero tambien pequeños proyectos pueden tener complejidades grandes.

[Inserta formula matematica] = C = Z Cp Tp

2.2 Symptoms of complexity (pg 19-20)
