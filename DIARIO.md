#Tarea 1.- Fork y configuración inicial <br/>
Un fork es una copia de un proyecto, que nos permite "trastear" sin que genere caos en el original<br/>
Y si quieres tener acceso a los cambios que se producen en el original mientras que usamos el fork, pues necesitaremos apuntar nuestro proyecto a ese original (mediante el upstream).
Una vez clonado con fork, nos aparece lo siguiente:
<img width="1853" height="1014" alt="imagen" src="https://github.com/user-attachments/assets/d946c505-f2ad-4b3d-86ec-e4b3dbb93418" /><br/>
Cuando hacemos el remote -v, comprobamos que tenemos nuestro fork correctamente y el original (upstream)<br/>
Captura 1.- Terminal con git remote -v mostrando origin y upstream <br/>
<img width="1253" height="114" alt="imagen" src="https://github.com/user-attachments/assets/77e8b645-0685-4b5e-97db-c6b8028925e7" />
Captura 2.- GitHub con la rama dev visible en el desplegable de ramas<br/>
<img width="958" height="716" alt="imagen" src="https://github.com/user-attachments/assets/6031efdc-be5d-4d12-a9d1-d4820c53f803" /><br/>
#Tarea 2.- Feature branch A: añadir la Opción 5 <br/>
El partir de la rama dev en lugar de la main es principalmente, para mantener estable la rama principal. Además, si hiciera falta aplicar un error importante en main, no arrastramos los cambios que no estén comprobados. <br/>
Captura 3.-La app en el navegador con la Opción 5 recién añadida
<img width="943" height="997" alt="imagen" src="https://github.com/user-attachments/assets/7f8ff0aa-85a5-481f-ab10-6976de7029c4" />
Y se comprueba que se ha subido bien la rama de esta opción 5 <br/>
<img width="943" height="997" alt="imagen" src="https://github.com/user-attachments/assets/431a206c-0934-4edd-8baf-29415a986eef" />
#Tarea 3.- Feature branch B: añadir la Opción 6 (aquí está el conflicto)<br/>
Un conflicto en git ocurre cuando se intentan aplicar varios cambios en la misma parte del código, y git no sabe cuál es "la buena". Nos pedirá que seamos nosotros los que decidamos qué es lo correcto. En nuestro ejemplo, en una rama (la 5) hemos puesto una cosa en el "description" de la opción 3 y otro "description" en la misma opción 3 en otra rama (la 6). Tendremos que decidir.<br/>
Comprobamos que la rama de la opción 6 está creada
<img width="943" height="997" alt="imagen" src="https://github.com/user-attachments/assets/65cbd574-479d-4dba-bfc8-8dfb12b324c1" /><br/><br/>
#Tarea 4 — Pull Request 1: Feature A a dev<br/>
En este punto revisé los cambios que se iban a producir en la rama dev, cuando añadiera las características de la rama feature/opcion-5. Esto es muy útil para comprobar que efectivamente lo que vamos a cambiar, es realmente lo que queremos cambiar. Además, nos da la posibilidad de que otros puedan comprobar dichos cambios antes de poder hacer el merge.<br />
Comprobamos que Github nos avisa de una Pull Request<br/>
<img width="940" height="319" alt="imagen" src="https://github.com/user-attachments/assets/fb872c0a-44d7-455c-9b6e-e8e875e2e5c0" /> <br/>
Captura 4. 	El PR de Feature A en GitHub con la pestaña Files changed abierta <br/>
<img width="940" height="1010" alt="imagen" src="https://github.com/user-attachments/assets/bcfe9d37-a07d-464c-a927-9a09fd20fc5e" /> <br/> <br/>
#Tarea 5 — Pull Request 2: Feature B a dev, conflicto<br/>
Los marcadores <<<<<<<, ======= y >>>>>>> nos indican que hay un conflicto al intentar hacer un Merge. Y debemos elegir con qué versión nos quedamos. En este caso, nos hemos quedado con la que indica que había un conflicto.<br/>
Captura 5: El PR de Feature B en GitHub mostrando el banner rojo de conflicto
<img width="887" height="1010" alt="imagen" src="https://github.com/user-attachments/assets/3bd306c3-a58d-4d85-b5f9-6cbf93122cd5" /><br/>
Captura 6:Los marcadores de conflicto (<<<<<<<, =======, >>>>>>>) en VS Code  <br/>
<img width="1557" height="989" alt="imagen" src="https://github.com/user-attachments/assets/c72db118-aaa9-463b-bc95-420892360156" /><br />
Captura 7:La app en el navegador con todas las opciones visibles tras resolver el conflicto<br />
<img width="885" height="1009" alt="imagen" src="https://github.com/user-attachments/assets/3fa220a7-1edb-45c3-83d3-f9cc053ea1b2" />
A continuación, se comprueba que el conflicto ya ha desaparecido: <br />
<img width="885" height="1009" alt="imagen" src="https://github.com/user-attachments/assets/7e2643b9-9044-4441-8282-95ac712143c8" />
#Tarea 6 — Limpieza y cierre del diario<br/>
<img width="1441" height="816" alt="imagen" src="https://github.com/user-attachments/assets/e45c739f-5e3e-403a-a94a-9a8a50ac8e6a" /> <br /><br />

CONCLUSIÓN:<br />
Me ha resultado muy interesante la actividad, aunque me ha costado un poco provocar el fallo. No había guardado los cambios del fichero en una de las ramas y me he "perdido" un poco. Pero he podido solucionarlo provocando el fallo nuevamente.







