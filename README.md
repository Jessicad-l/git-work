# git-work

<center>

# GIT-WORK


</center>

***Nombre:*** Jessica Dóniz Linares, David Gutiérrez Gutiérrez </br>
***Curso:*** 2º de Ciclo Superior de Desarrollo de Aplicaciones Web.

### ÍNDICE

+ [Introducción](#id1)
+ [Objetivos](#id2)
+ [Material empleado](#id3)
+ [Desarrollo](#id4)
+ [Conclusiones](#id5)


### ***Introducción***. <a name="id1"></a>

En la siguiente práctica trabajaremos con documentación y el sistema de control de versiones de github. </br>
</br>El sistema de control de versiones nos permite llevar un seguimiento de los cambios realizados, no solo eso, sino que también te ofrece la posibilidad de volver a versiones anteriores. Este sistema te permite trabajar de manera simultánea con diferentes colaboradores, pudiendo contrastar las diferentes versiones de los usuarios.


### ***Objetivos***. <a name="id2"></a>

Los objetivos a realizar son:

+ Crear un repositorio
+ Clonar el repositorio en local
+ Crear ramas y moverse entre ellas
+ Crear issues y solucionarlas
+ Modificar los archivos y subirlos
+ Hacer y revisar los pull request antes del merge
+ Arreglar conflictos entre diferentes ramas

### ***Material empleado***. <a name="id3"></a>

Para realizar esta actividad hemos empleado:

*Hardware*
+ Ordenadores de clase
+ Ordenadores de casa

*Software*
+ Github
+ Máquina virtual (Debian)

### ***Desarrollo***. <a name="id4"></a>

***user1:*** David Gutiérrez Gutiérrez </br>
***user2:*** Jessica Dóniz Linares

1. user1 creará un repositorio público llamado git-work en su cuenta de GitHub, añadiendo un README.md y una licencia MIT.

   Creamos el repositorio git-work desde el github con el README.md y con la licencia MIT.

1. user1 clonará el repo y añadirá los ficheros: index.html, bootstrap.min.css y cover.css. Luego subirá los cambios al upstream. 

   user1 clona el repositorio -> `git clone https://github.com/DavidGG2004/git-work.git`

2. user2 creará un fork de git-work desde su cuenta de GitHub.



3. user2 clonará su fork del repo.

   user2 clona el fork del repositorio git-work -> `git clone https://github.com/Jessicad-l/git-work.git`

4. user1 creará una issue con el título "Add custom text for startup contents".



5. user2 creará una nueva rama custom-text y modificará el fichero index.html personalizándolo para una supuesta startup.

   user2 crea la rama custom-text y se mueve hacia ella para modificar el index.html -> `git checkout -b custom-text`
   Modifica el fichero index.html y commitea los cambios-> 
   ```
   nano index.html
   git add index.html
   git commit -m "Starting index.html startup project"
   git push origin custom-text
   ```
   
8. user2 enviará un PR a user1.

Envía un pull request con los cambios realizados ->
   
10. user1 probará el PR de user2 en su máquina (copia local) creando previamente un remoto denominado upstream, y realizará ciertos cambios en su copia local que luego deberá subir al propio PR.

   user1 prueba el pull request creando upstream -> 
   ```
   git remote add upstream https://github.com/Jessicad-l/git-work.git
   git fetch upstream
   git checkout -b custom-text upstream/custom-text
   ```

11. user1 y user2 tendrán una pequeña conversación en la página del PR, donde cada usuario incluirá, al menos, un cambio más.



12. user1 finalmente aprobará el PR, cerrará la issue creada (usando una referencia a la misma) y actualizará la rama principal en su copia local.



13. user2 deberá incorporar los cambios de la rama principal de upstream en su propia rama principal.



14. user1 creará una issue con el título "Improve UX with cool colors".



15. user1 cambiará la línea 10 de cover.css a: color: purple;



16. user1 hará simplemente un commit local en main → NO HACER git push.



17. user2 creará una nueva rama cool-colors y cambiará la línea 10 de cover.css a: color: darkgreen;



18. user2 enviará un PR a user1.



19. user1 probará el PR de user2 (en su copia local). A continuación tratará de mergear el contenido de la rama cool-colors en su rama principal y tendrá que gestionar el conflicto: Dejar el contenido que viene de user2.



20. Después del commit para arreglar el conflicto, user1 modificará la línea 11 de cover.css a: text-shadow: 2px 2px 8px lightgreen;



21. user1 hará un commit especificando en el mensaje de commit el cambio hecho (sombra) y que se cierra la issue creada (usar referencia a la issue). A continuación subirá los cambios a origin/main.



22. user1 etiquetará esta versión (en su copia local) como 0.1.0 y después de subir los cambios creará una "release" en GitHub apuntando a esta etiqueta.




Si encontramos dificultades a la hora de realizar algún paso debemos explicar esas dificultades, que pasos hemos seguido para resolverla y los resultados obtenidos.

### ***Conclusiones***. <a name="id5"></a>

En esta parte debemos exponer las conclusiones que sacamos del desarrollo de la prácica.
