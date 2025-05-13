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

También se pueden añadir todos los archivos del directorio actual al staging area usando asterisco:

```bash
#Inicializa el repositorio local Git

git add *

```

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


---

# Conexión de Git y GitHub

A partir de este punto se aconseja instalar WSL si estás en Windows para ejecutar comandos de Ubuntu en terminal. Por tanto, la gran parte de los pasos es la misma en Linux (distribuciones basadas en Debian como Ubuntu o Mint), y Windows con WSL. En ambos casos se usará la terminal, cuidando que la terminal en Windows sea la de WSL Ubuntu y no el Powershell nativo de Windows.



## Creando directorio para los datos de conexión

Para conectar el repositorio local con un repositorio de GitHub, usaremos la conexión SSH, para lo cual necesitamos una clave RSA. Primero, en el directorio home de WSL de tu usuario en tu computadora (`~` o `/home/you_user` en Linux, la misma ruta en WSL Windows) crea una nueva carpeta <b>~/.ssh</b>, y abre la terminal dentro de ella. Puedes hacerlo con los siguientes comandos:

```bash
#Cambiar al home de tu usuario
cd ~
#Crear directorio
mkdir .ssh
#Entrar al directorio
cd .ssh
```

Es importante usar la ruta `~` del WSL en vez de tu carpeta de usuario personal en Windows (comunmente `C:\Users\your_user`) pues sólo puedes gestionar permisos con comandos de Unix dentro de los directorios de WSL, no en los nativos de Windows.


## Creación de la llave RSA

Ejecuta el siguiente comando para generar una llave RSA:

```bash
ssh-keygen -N "passphrase"
```

El argumento adicional `-N "passphrase"` es opcional y por tanto se puede omitir, sirve para crear la llave usando una frase o palabra secreta (puedes usar la que quieras en vez de `"passphrase"`) como semilla generadora, pero la llave puede crearse sin usar una palabra secreta. Por mayor seguridad, se recomienda usar la passphrase, de este modo, las futuras conexiones la pedirán siempre que se haga una consulta con GitHub, sirviendo como una contraseña.

Al ejecutar el comando, pedirá que se ingrese un nombre para el archivo de la clave, puedes poner el que sea, por ejemplo, `my_key1`, y dicha clave se guardará en la carpeta <b>.ssh</b> donde estás ejecutando el comando. Si vas a la carpeta, verás que se han generado dos archivos, `my_key1` (sin extensión, pero puede abrirse con cualquier editor de texto plano como Bloc de Notas), el archivo de clave privada, y que por tanto no debe compartirse; y `my_key1.pub`, el archivo con la clave pública de cifrado. También puedes comprobar esto listando los archivos del directorio actual:

```bash
ls -a
```

## Configurando el Host

Dentro de la carpeta <b>.ssh</b> (todavía) debes crear un archivo llamado `config`, el cual abrimos con Bloc de Notas (o equivalentes en Linux) o también con Code, y agregamos lo siguiente:

```text
#Primer host
Host github-host1
  HostName github.com
  User git
  IdentityFile ~/.ssh/my_key1
```

En donde puedes cambiar "github-host1" por cualquier nombre que quieras, pero se recomienda uno alusivo al repositorio (éste) y usuario (tú) para distinguirlo de cualquier otra conexión SSH, o de cualquier conexión a otro repositorio GitHub por parte de otros usuarios en el equipo. De igual modo, en la línea de `IdentityFile` debes cambiar `my_key1` por el nombre de archivo que le pusiste a tu clave privada. Si se requiriera añadir más usuarios que se conecten ya sea a éste o a otros repositorios GitHub, se pueden copiar las líneas anteriores por cada usuario y añadirlas al archivo `config`, siempre y cuando los nombres del `Host` sean distintos para cada uno. Un ejemplo de `config` para dos usuarios sería el siguiente:

```text
#Primer host (para el primer usuario)
Host github-host1
  HostName github.com
  User git
  IdentityFile ~/.ssh/my_key1

#Segundo host (para el segundo usuario)
Host github-host2
  HostName github.com
  User git
  IdentityFile ~/.ssh/my_key2
```

Ahora, hay un paso extra en Windows. Dado que el entorno simulado de Ubuntu WSL no puede cambiar los permisos de acceso de los documentos de Windows, debes copiar los archivos de la carpeta <b>.ssh</b> (que en Windows está ubicada en `C:\Users\Tu usuario\.ssh`) a una carpeta dentro del sistema de archivos de Ubuntu WSL, la carpeta `~/.ssh`. Para ello, basta con abrir la terminal dentro del <b>.ssh</b> original del sistema de archivos de Windows y ejecutar:

```bash
cp * ~/.ssh
```

Si en un futuro modificas alguno de los archivos (por ejemplo, `config`), toma en cuenta que el cambio sólo se verá reflejado en Windows, por lo que tendrías que copiar nuevamente el archivo actualizado, cambiando el asterisco * por el nombre del archivo a copiar en el sistema Ubuntu WSL. Por ejemplo, para `config`:

```bash
cp config ~/.ssh
```

Una vez hecho esto, debes moverte dentro de la terminal al directorio `~/.ssh` de Ubuntu, lo cual se hace con:

```bash
cd ~/.ssh
```

El paso anterior aplica tanto en Windows como en Linux, y a partir de aquí los pasos son aplicables en ambos sistemas, siempre y cuando la terminal esté abierta dentro de `~/.ssh` (lo cual aseguras ejecutando el paso anterior). Para que la conexión SSH funcione, se requiere que el archivo de clave privada sólo tenga permisos de acceso para el propietario del archivo. Para asegurar estos permisos, se debe ejecutar:

```bash
chmod 600 my_key1
```

Ahora, debes abrir este repositorio en GitHub, ya sea desde la cuenta de LINX, o desde tu cuenta personal una vez que el dueño del repositorio (la cuenta de LINX) te haya dado los permisos para editarlo. Dentro del repositorio, ve a `Settings`, y luego en el menú del lado izquierdo ve a `Deploy Keys`. Dale a `Add deploy key`, y en el recuadro `Key` pega la clave que aparece dentro del archivo de llave pública `my_key1.pub` (puedes abrir el archivo con el Bloc de Notas, seleccionar todo `Ctrl+A` y luego copiar `Ctrl+C`). Bajo ninguna circunstancia debes pegar la clave privada que aparece en el archivo sin extensión `my_key1`. Finalmente, agrega algún título alusivo en el recuadro `Title` en GitHub y dale a guardar la llave.

Con las claves (pública y privada) y el archivo `config` en la carpeta correcta `~/.ssh`, y los permisos adecuados para la llave privada, ya se puede iniciar sesión mediane SSH:

```bash
ssh -T -F ~/.ssh git@github-host1
```

En donde el parámetro `-T` indica que la conexión se efectúa sin el modo de (pseudo)terminal activado, lo cual es necesario en GitHub ya que no vamos a usar comandos de Bash en el servidor remoto (GitHub); el parámetro `-F ~/.ssh` es opcional y sirve para indicar la ruta del archivo `config`, si se omite toma por defecto la ruta `~/.ssh` (aún así recomendamos usarlo en sistemas Windows con WSL, para evitar confusión entre el <b>.ssh</b> de Windows y el de Ubuntu), y finalmente se escribe el nombre de usuario `git` (para hacer push en Git siempre se debe usar este nombre) seguido de un arroba y el host que especificaste en el `config`. Posteriormente el programa te pedirá que ingreses la passphrase con la que creaste la llave asignada al host, y al ingresarla se iniciará la sesión. Si más de un usuario se requiere conectar a sus respectivos repositorios de GitHub en el mismo equipo, basta con repetir el comando anterior, pero cambiando el nombre del host (después del arroba) por el host asignado a ese repositorio. Por ello es importante el archivo `config` con distintos Hosts.


<h2>Enlazando un repositorio a un Host</h2>

Los pasos anteriores sólo sirven para establecer la conexión desde el PC local a GitHub, pero ahora se debe enlazar el repositorio local con algún host en `config` (por ejemplo, `github-host1`). Para ello, se abre la carpeta oculta `.git` del repositorio local (esta carpeta se crea automáticamente al ejecutar `git init`), y luego se abre el archivo `config` de ese Git (no confundir con el `config` de <b>.ssh</b>). Ahora, se debe buscar la sección que contiene los datos del repositorio remoto:

```text
[remote "origin"]
	url = github-host1:your_user/your_repo.git
	fetch = +refs/heads/*:refs/remotes/origin/*
```

En la línea de `url` se debe cambiar el `github-host1` por el nombre que asignaste al Host en SSH, y `your_user/your_repo.git` es el nombre del usuario propietario en GitHub seguido del nombre del repositorio donde estás trabajando. En el caso de este repositorio, debe usarse `LINX-ICN-UNAM/GroundStation.git`. Tras esto, cualquier push que se haga mediante Git será enviado a GitHub mediante el host personalizado `github-host1` creado en el paso anterior, el cual ya tiene asignada la misma llave de acceso que cargaste en el repositorio remoto GitHub con DeployKeys. Ahora, ya se puede ejecutar el primer push, sólo ve a la carpeta del proyecto donde inicializaste Git, abre una terminal ahí mismo y ejecuta:

```bash
git push -u -f origin main
```

Si creaste la llave RSA con una passphrase, cada vez que hagas push se te pedirá de nuevo. Esto agrega una capa de seguridad para que usuarios no autorizados con acceso al equipo no intenten mandar código hacia este repositorio, o simplemente que no lo manden aquí por error confundiéndolo con su repositorio (en caso de haber más de una persona usando GitHub en el mismo equipo).



