# GIT & Github Course (Windows)
Repositorio de aprendizaje sobre GIT & Github.


## 📑 Índice

- [Recursos](#recursos)
- [Downloads](#downloads)
- [Instalacion GIT](#instalacion-git)
   - [Instalación por descarga de archivo](#instalación-por-descarga-de-archivo)
   - [Instalación en consola](#instalación-en-consola)
   - [Comprobar instalación de GIT](#comprobar-instalación-de-git)
- [Comandos básicos](#comandos-básicos)
   - [git --version](#git---version)
   - [git -help](#git---help)
- [Comandos básicos en la Terminal Linux, CMD, PowerShell, Git Bash](#comandos-básicos-en-la-terminal-linux-cmd-powershell-git-bash)
- [Configuración de GIT](#configuración-de-git)
   - [Configuración Global (Nombre de usuario, Email)](#configuración-global)
- [git init](#git-init)
- [Ramas en git (Branches)](#ramas-en-git)
   - [Git status](#git-status)
- [Git add y commit](#git-add-y-commit)
   - [Git add](#git-add)
   - [Git commit](#git-commit)
- [Git log y git status](#git-log-y-git-status)
---

## recursos

* [Git Website](https://git-scm.com/) - Website Git, Download
* [Git Book](https://git-scm.com/book/en/v2) - Git Book.
* [Git Documentation](https://git-scm.com/doc) - Git Documentation.

---

## downloads

 * [Windows](https://git-scm.com/downloads/win)
 * [Linux](https://git-scm.com/downloads/linux)
 * [macOS](https://git-scm.com/downloads/mac)

---

## Instalacion GIT  
La instalación puede hacer de dos formas.
1. Instalador por descarga de archivo.
2. Comando en la terminal.

## Instalación por descarga de archivo.
* Descargando el archivo y ejecutandolo con doble click.

## Instalación en consola
* Agregar en el simbolo del sistema de nuestro ordenador el siguiente comando. 

```bash
winget install --id Git.Git -e --source winget
```

Se desplegará la siguiente ventana de instalación.

![image](https://github.com/user-attachments/assets/caf889f4-7dc0-4c6d-a8fa-ec187927825d)

Finalizará la instalación.

![image](https://github.com/user-attachments/assets/49d690ab-36e2-4bdb-8063-33f9cfa1084a)

## Comprobar instalación de git
Ingresar el siguiente comando en la terminal
```bash
git
```
Saldrá lo siguiente junto con algunos comandos:  

![image](https://github.com/user-attachments/assets/6e09e8ce-bb90-407e-981a-1da6f35cf583)

---

## Comandos básicos.  
Estos son algunos comandos en terminal básicos para cualquiere terminal compatible con GIT.


### *git --version*  
_Este comando sirve para la ver la versión que tenemos instalada en nuestra PC._
```bash
git --version
```  
También podemos usar un comando más simple.
```bash  
git -v
```
![image](https://github.com/user-attachments/assets/182253f9-a29d-4843-a489-fe970eca827d)

### *git --help* 
_Este comando sirve para visualizar todos los comandos y su descripción disponibles en GIT._
```bash  
git --help
```
![image](https://github.com/user-attachments/assets/43ef83a5-0011-40a6-b2f4-adbce88c7654)

## Comandos básicos en la Terminal Linux, CMD, PowerShell, Git Bash.

Esta es una tabla con los comandos equivalentes entre (Linux, CMD, PowerShell, Git Bash) :

| Acción                          | Linux/macOS       | CMD (Windows)     | PowerShell         | Git Bash           |
|---------------------------------|-------------------|-------------------|--------------------|--------------------|
| Listar archivos                 | `ls`              | `dir`             | `ls` (alias)       | `ls`               |
| Cambiar de directorio          | `cd carpeta`      | `cd carpeta`      | `cd carpeta`       | `cd carpeta`       |
| regresar carpeta                | `cd ..`           | `cd ..`           | `cd ..`            | `cd ..`            |
| Mostrar ruta actual            | `pwd`             | `cd`              | `pwd`              | `pwd`              |
| Limpiar la pantalla            | `clear`           | `cls`             | `Clear-Host` o `cls` | `clear` o `cls`    |
| Eliminar un archivo            | `rm archivo.txt`  | `del archivo.txt` | `Remove-Item archivo.txt` | `rm archivo.txt`   |
| Copiar un archivo              | `cp a.txt b.txt`  | `copy a.txt b.txt`| `Copy-Item a.txt b.txt` | `cp a.txt b.txt`   |
| Mover o renombrar un archivo   | `mv a.txt b.txt`  | `move a.txt b.txt`| `Move-Item a.txt b.txt` | `mv a.txt b.txt`   |
| **Crear una carpeta**          | `mkdir nueva_carpeta` | `mkdir nueva_carpeta`   | `mkdir nueva_carpeta` o `New-Item -Type Directory -Name nueva_carpeta` | `mkdir nueva_carpeta` |

#### 💡 Recomendaciones

- **Git Bash** es ideal si vienes de Linux o estás usando Git en Windows.
- **PowerShell** es más potente que CMD y permite scripts avanzados.
- **CMD** es básico pero sigue siendo útil para tareas simples.

---

## Configuración de GIT
### Configuración global. 
   Esta configuración afectará a nivel usuario en la pc en la que nos encontremos.
   * **Nombre de usuario:**  
     Estableceremos un nombre de usuario para GIT a nivel global en nuestra PC. 

```bash  
git config --global user.name "[tu_usuario]"
```
En la carpeta de usuario de nuestra PC creará el siguiente archivo.  

![image](https://github.com/user-attachments/assets/432e49f3-cea5-4341-b022-d6f78de38fca)  

Al abrirlo con un block de notas nos mostrará lo siguiente:  

![image](https://github.com/user-attachments/assets/79e75383-e181-4d38-9f29-4fa005e50599)

   * **Email de usuario**  
     Estableceremos un Email de usuario para nuestra PC.

```bash  
git config --global user.email "[tu_email]"
```
Al abrir el archivo de nuevo aparecerán nuestras credenciales de usuario.  

![image](https://github.com/user-attachments/assets/1681ea38-b15a-4d77-8f1e-d80724ae99b6)

Con esto tendremos las configuraciones necesarias para usar GIT.

---

## git init

Dirigirse a la carpeta raiz del directo a tráves de CMD y escribir el siguiente comando:  

```bash  
git init
```

Por ejemplo
```bash  
C:\Users\addi_\Documents\GIT>git init
```
A continuación nos mostrará un mensaje que se ha creado un repositorio vacío.  
![image](https://github.com/user-attachments/assets/a4509bc4-e84f-4f40-ab0d-5ad37d33b7a4)  

Si nos dirigimos a la carpeta veremos que se ha creado el archivo .git.  
![image](https://github.com/user-attachments/assets/26d87983-b104-415c-bf3c-b3651c69c83d)

---

## Ramas en GIT  
Para poder trabajar en un proyecto es necesario trabajar con diferentes ramas.
Para nombrar una a la rama principal es necesario agregar el siguiente comando:  
```bash  
git branch -m main
```
Aparentemente no aparece un cambio pero el nombre de la rama se actualizó a main.  
![image](https://github.com/user-attachments/assets/1af0e088-8a30-4e4b-a1fb-fd5c6fc15b70)

### Git status
Para saber si estoy en la rama principal agregar el siguiente comando:  
```bash  
git status
```  
![image](https://github.com/user-attachments/assets/6c8ac580-0ed8-4d54-8076-7fbf13bb15e4)  
Aparece la leyenda "On branch main" lo cual nos indica que estamos en la rama principal.

---

## git add y commit  
Para iniciar debemos ver el estado de nuestro proyecto agregado el siguiente comando:
```bash  
git status
```
![image](https://github.com/user-attachments/assets/6f73c98f-fc47-45fa-be66-cfd11daf3494)  

### Git add

Veremos que estamos en la rama principal y tenemos un archivo de prueba marcado en rojo.
Al momento ese archivo aun no está agregado a GIT, así que lo agregaremos con el comando:  

```bash  
git add helloworld.py
```

para verificar que se agregó correctamente consultamos de nuevo con [git status](#git-status):  
```bash  
git status
```
![image](https://github.com/user-attachments/assets/20d73e72-d9bb-4c6e-849c-ea30291aeae3)  
Podremos darnos cuenta que ya está en verde, esto significa que ya el stage ya lo tomó en cuenta pero aun es necesario hacer commit.

### Git commit

Agregamos el siguiente comando:  
```bash  
git commit
```
Enseguida nos aparecerá la siguiente ventana:  
![image](https://github.com/user-attachments/assets/e3840145-155d-4727-bc11-3d9886c6b3fd)  

Es necesario agregar un nombre en la parte superior del mensaje:  
![image](https://github.com/user-attachments/assets/e69b1a5f-0353-4185-a709-e487db7da006)  

Existe otra forma de hacerlo con el siguiente comando.
```bash  
git commit -m "[Mensaje al crear el commit]"
```
En este caso usaremos el siguiente:  
```bash  
git commit -m "Este es mi primer commit"
```
Dandonos como resultado lo siguiente:  
![image](https://github.com/user-attachments/assets/9cfd0e1f-e197-4bec-9d13-5d5f05568eb9)  
Si analizamos podremos ver la rama en la que se encuentra, su identificador unico, así como los archivos que se han modificado.  

Al revisar de nuva cuenta con [git status](#git-status) podremos ver lo siguiente:  

![image](https://github.com/user-attachments/assets/451b3fd4-30fc-4e43-ba3d-4d890f3f2d26)

---

## git log y git status
