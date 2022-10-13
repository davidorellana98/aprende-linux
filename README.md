<h1 align="center">Comandos de Linux</h1>

![portada](https://raw.github.com/davidorellana98/aprende-linux/main/images/portadalinux.png)

- **Comandos de ayuda**

```xml
help <nombre del comando>
- o -
<nombre del comando> --help

// Ejemplo

help cd
- o -
cat --help
```
Estos comandos te ayudarán a saber otras opciones que existen en un comando en especifico (toda la información será presentada en la terminal).

- **Comandos de limpieza y salida de la terminal**

```xml
clear
- o -
ctrl + l // Windows
```
Estos comandos te permiten tener limpia la terminal.

```xml
exit
```
Este comando te permite salir de la terminal.

- **Comandos para ver rutas y características de archivos y directorios**

```xml
pwd
```
Este comando te permite ver la ruta especifica donde te encuentras actualmente.

```xml
find -name "<nombre del archivo o directorio>"

// Ejemplo

find -name "index.html"
```
Este comando te permite saber la ruta exacta, donde se encuentra dicho archivo o directorio.

```xml
find -iname "<nombre del archivo o directorio>"

// Ejemplo

find -iname "tEsT"
```
Este comando va ignorar las letras mayúsculas o minúsculas en la búsqueda de cierto archivo o directorio.

```xml
ls
```
Este comando te permite ver el listado de los archivos y directorios en el lugar que te encuentras actualmente.

```xml
ls -l 
- o - 
ls -lh
```
Estos comandos te permiten ver el listado de archivos y directorios con información más especifica, como es la hora y fecha de su última modificación.

```xml
ls -a
```
Este comando te permite ver el listado de archivos y directorios generales y ocultos.

```xml
ls -s
```
Este comando te permite ver el listado de archivos con su peso en memoria que tiene actualmente.

```xml
ls -r
```
Este comando te permite ver el listado de archivos y directorios de manera descendente hasta ascendente.

- **Comandos para direccionarse a un directorio**

```xml
cd
```
Este comando te direccionara al home, donde estará toda la cabecera raíz del sistema.

```xml
cd <nombre del directorio>

// Ejemplo

cd aprende-linux
```
Este comando te permite abrir un directorio y poder interactuar con dicho directorio (no permite abrir archivos).

```xml
cd ..
```
Este comando te permite retroceder un paso, en la navegación de directorios.

```xml
cd -
```
Este comando te permite regresar al lugar que estabas anteriormente de manera automática, es útil cuando cuando has cambiado a un directorio largo y no te acuerdas su ruta de llegada.

- **Comandos para crear archivos y directorios**

```xml
mkdir <nombre del directorio>

// Ejemplo

mkdir aprende-linux
```
Este comando te permite crear directorios, teniendo en cuenta que si ingresa espacios creara otro directorio adicional.

```xml
touch <nombre del archivo>

// Ejemplo

touch style.css
```
Este comando te permite crear archivos o varios archivos con extensiones, por ejemplo: test.txt, web.html, entre otras.

- **Comandos para ver el contenido y características de un archivo**

```xml
file <nombre del archivo>

// Ejemplo

file prueba.txt
```
Este comando describe las características del tipo de archivo a analizar.

```xml
echo "<cadena de caracteres>" > <nombre del archivo>

// Ejemplo

echo "hola mundo" > holaMundo.txt
```
Este comando te permite crear mensajes desde la terminal, para posteriormente sobrescribir el mensaje del archivo, si el archivo no existe lo creara automáticamente.

```xml
echo "<cadena de caracteres>" >> <nombre del archivo>

// Ejemplo

echo "hola mundo" >> holaMundo.txt
```
Este comando te permite crear mensajes desde la terminal para pasarlos a un archivo, concatenándolo con el mensaje anterior, que tenía en su archivo.

```xml
cat <nombre del archivo>

// Ejemplo

cat test.js
```
Este comando te permite visualizar el contenido que tiene el archivo seleccionado, es muy útil para ver contenidos muy breves.

```xml
cat -n <nombre del archivo>

// Ejemplo

cat -n test.js
```
Este comando te permite visualizar el contenido del archivo especificando en su costado el número de líneas que están presentes.

- **Comandos para mover y copiar archivos y directorios**

```xml
mv <nombre del directorio o archivo que se va a mover> <nombre del directorio donde se va a mover>

// Ejemplo

mv uno.txt directorio-dos
```
Este comando te permite mover un directorio o archivo a otro directorio, especificando el lugar que se desea mover. Además si mueve dos archivos, el archivo que se coloco ultimo será el que perdure con su nombre actual, no importa el formato de extensión en el que lo va a renombrar.

```xml
cp <nombre del archivo que se va a copiar> <nombre del directorio donde se va a copiar el archivo>

// Ejemplo

cp uno.txt directorio-dos
```
Este comando te permite copiar un archivo y destinarlo a un directorio en especifico. También puedes renombrar el nombre del archivo sin perder su información.

```xml
cp -r <nombre del directorio que se va a copiar> <nombre del directorio donde se va a copiar>

// Ejemplo

cp -r directorio-uno directorio-dos
```
Este comando te permite copiar el contenido que hay en un directorio y trasladarla a un nuevo directorio (si la carpeta no existe, la creara automáticamente).

- **Comandos para borrar archivos y directorios**

```xml
rm <nombre del archivo>

// Ejemplo

rm index.html
```
Este comando te permite borrar un archivo (no borra carpetas o directorios).

```xml
rm -i <nombre del archivo>

// Ejemplo

rm -i index.html
```
Este comando te lanzara un mensaje si desea o no borrar dicho archivo; para poder borrar el archivo se colocara la palabra [yes] y si no desea borrarlo colocara la letra [n].

```xml
rm -r <nombre del archivo o directorio>

// Ejemplo

rm -r aprende-linux
```
Este comando te permite borrar archivos y además directorios.

- **Comandos para crear comandos personalizados**

```xml
alias
```
Este comando te permite ver el listados de alias que se han creado.

```xml
alias <nombre del alias>="<nombre del comando>"

// Ejemplo

alias regresar="cd .."
```
Este comando te permite colocar un nombre personalizado a cierto comando en particular.

```xml
unalias <nombre del alias creado>

// Ejemplo

unalias regresar
```
Este comando te permite borrar un alias creado con anterioridad.

- **Comando para abrir un archivo en un editor de texto**

```xml
vim <nombre del archivo>

// Ejemplo

vim README.md
```
Este comando abrirá el editor de texto llamado VIM, con el contenido que tiene dicho archivo. Para poder escribir y salir del editor, sigue los siguientes pasos:
1. Presione (**i**) para comenzar a escribir en el editor.
2. Presione (**esc**) para dejar de escribir.
3. Inserte (**:wq**) para guardar lo escrito y poder salir.

## Contribuye con un comando 🤝

Sabemos que el trabajo en equipo, es mucho más eficaz y tiene un mayor número de resultados, por eso te animo a que puedas contribuir con algunas correcciones del repositorio o algún comando adicional de Git, haciendo un **pull request** a este repositorio de Github.

Cada pull request que realices te ayudara a crecer como programador o programadora y además poder ayudar a miles de personas a saber más de los comandos de Git ❤️

Si te ha parecido útil este repositorio apóyalo con una estrellita ⭐

## Licencia

Consulte el archivo [LICENSE](https://github.com/davidorellana98/aprende-linux/blob/main/LICENSE.md) para conocer los derechos y limitaciones de la licencia (Creative Commons).
