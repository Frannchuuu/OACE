
UNIDAD 3. ACTIVIDAD 2. EJERCICIOS CON FICHEROS
crea un directorio llamado SMM en la raíz de la Unidad C. Dentro de ese directorio haz lossiguientes ejercicios:

"<img width="448" height="417" alt="imagen" src="https://github.com/user-attachments/assets/95f00ff7-5e27-40ae-bfaf-1a2fed412c75" />

_1.- Situado en smm crea los directorios A, B, C y D. Utiliza trayectoria absoluta._
```
c:\smm>md c:\smm\A,B,C,D
```
"<img width="90" height="333" alt="imagen" src="https://github.com/user-attachments/assets/c1755b3a-22d0-4361-a758-c6c7e52d8fc5" />

_2.- Sitúate en D y desde allí crea A1, A2, A21, A22, A221 con una única sentencia utilizandotrayectoria relativa._
```
c:\smm\D>md ..\A\A1 ..\A\A2\ ..\A\A2\A21 ..\A\A2\A22\A221 
```
<img width="229" height="114" alt="imagen" src="https://github.com/user-attachments/assets/c9207375-c414-4969-9e40-cca25bb208b2" />

_3.- Sitúate en A221 y desde allí crea B1, B11, B111, B112 con una única sentencia y utilizandotrayectoria relativa._
```
c:\smm>cd A\A2\A22\A221

c:\smm\A\A2\A22\A221>

c:\smm\A\A2\A22\A221>md ..\..\..\..\B\B1\B11\B111 ..\..\..\..\B\B1\B11\B112 
```
<img width="229" height="97" alt="imagen" src="https://github.com/user-attachments/assets/e4022f05-8d86-4132-afef-97fb8becdb0e" />

_4.- Estando situado en A221, crea un fichero llamado líneas.txt en el directorio C que contenga elárbol de directorios dependiente del directorio A (incluyendo los subdirectorios)._
```
C:\smm\A\A2\A22\A221>tree c:\smm\A > c:\smm\c\lineas.txt 
```
<img width="241" height="113" alt="imagen" src="https://github.com/user-attachments/assets/db24d26d-c42e-43c4-a0a4-a3368f8e180a" />

5.- Crea en D un fichero llamado Nombre.txt que contenga tu nombre y otro fichero llamado Apellido.txt que contenga tu primer apellido.
```
C:\smm\A\A2\A22\A221> > c:\smm\D\Nombre.txt

C:\smm\A\A2\A22\A221> > c:\smm\D\Apellido.txt 
```
<img width="407" height="397" alt="imagen" src="https://github.com/user-attachments/assets/5cc9c34a-278d-4e5d-921f-9be6d5483b43" />

6.- Genera un fichero llamado union.txt en D que contenga el contenido de Nombre.txt y Apellido.txt 
```
C:\smm\D>type nombre.txt >> union.txt

C:\smm\D>type apellido.txt >> union.txt
```
<img width="311" height="205" alt="imagen" src="https://github.com/user-attachments/assets/a2f5b74e-88f2-4db3-9f73-785e56589e72" />

7.- Mueve el fichero union.txt a A21.
```
C:\smm\D>move union.txt ..\A\A2\A21\
```
<img width="407" height="397" alt="imagen" src="https://github.com/user-attachments/assets/fa56a122-04b5-4960-b1e7-f8b411ab5945" />

8.- Mueve el directorio A2 dentro de C.
```
move C:\smm\A\A2 c:\smm\C\
```
**<img width="407" height="93" alt="imagen" src="https://github.com/user-attachments/assets/57fbe764-b387-49dd-92e1-8e0059a9405a" />
**
