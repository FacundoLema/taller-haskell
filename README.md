# Taller de Algebra I #

## Test de funciones ###

**Tester** es un script (no oficial) para verificar la validez de las funciones dadas como tarea en cada clase del taller de Algebra I. Lo unico que hace **Tester** es ejecutar las funciones con diferentes parámetros y verificar si la respuesta es la esperada. **Tester** viene en tres formas distintas, dependiendo la plataforma en la que se quiera utilizar:
- **PowerShell** (Windows 7+ | PowerShell Core 6+)
- **Bash** (Linux, macOS, *nix)

### ¿Cómo lo descargo? ### 
`requiere git`

```
git clone https://github.com/FacundoLema/taller-haskell.git
cd taller-haskell
rm -r clases
rm -r img
```
*altrernativamente, se puede descargar el archivo ZIP desde GitHub usando el boton verde*

### ¿Como lo uso? ###
- Copiá y pegá en la carpeta *(taller-haskell)* el archivo de Haskell que quieras chequear.

- Abrí la terminal y navegá a *taller-algebra*. Si usas Windows, usa **PowerShell**.

**Tester** toma dos argumentos, ***-a*** y ***-c***. Adicionalmente, se puede especificar una flag: ***-m***
- ***-a*** : nombre del archivo de Haskell que copiaste y pegaste en la carpeta, incluida su extensión (.hs). 
- ***-c*** : número de la clase a la cual corresponden los ejercicios. Solo acepta números (int).*
- ***-m*** es una flag. Si las funciones estan definidas dentro de un módulo (es decir, si al comienzo de tu archivo escribiste *module ModuleName where*), tenes que usarla. Es importante que el nombre del módulo comience con mayúscula (requisito de Haskell) y que el nombre del módulo sea exactamente igual al nombre del archivo.

Ejecutá, reemplazando por el nombre de tu archivo y el número de clase:
```
.\tester.ps1 -a archivo.hs -c n     # PowerShell - Windows
```
```
.\tester.sh -a archivo.hs -c n      # Bash - Linux
```
O, si tus funciones están definidas dentro de un módulo:
```
.\tester.ps1 -a archivo.hs -c n -m     # PowerShell - Windows
```
```
.\tester.sh -a archivo.hs -c n -m      # Bash - Linux
```