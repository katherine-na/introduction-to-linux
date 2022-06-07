## Sistemas Operativos.

El **software** (programa) se encarga de gestionar y usar el **hardware** (piezas). Interactua con la red de circuitos y componentes del ordenador.
**Ejemplos de Software**

- Windows
- Mac OS
- Linux

## Propiedades de Linux.

| Libre           | Su código fuente se puede usar, modificar y distribuir               |
| :-------------- | :------------------------------------------------------------------- |
| Multiusuario    | Varios usuarios pueden trabajar concurrentemente en la misma maquina |
| Multiplataforma | Instalable el multitud de dispositivos                               |
| Redes           | Permite acceso a recursos remotos y comunicaciones                   |
| Estabilidad     | Funciona correctamente meses, incluso años                           |
| Multitarea      | Se pueden realizar distintas tareas a la vez                         |

## Software libre.

**Libertades del software libre**

- Libertad de usar el programa.
- Estudiar cómo funciona el programa y modificarlo
- Libertad de distribuir copias del programa

## Qué es Linux?

Es un sistema operativo, formado por:

| Nucleo (Kernel)         | Interactua directamente con el hardware             | Gestion de memoria, control de acceso al ordenador y permisos |
| :---------------------- | :-------------------------------------------------- | :------------------------------------------------------------ |
| **Shell**               | **Intérprete de lenguaje de comandos**              | **Ejecuta los comandos**                                      |
| **Sistema de archivos** | **Unidad básica de organización de la información** | **Sin restricciones sobre nombre, extenciones, etc**          |

### Utilidad y aplicaciones.

- Edición y procesamiento del texto.
- Lenguajes y entornos de programación.
- Bases de datos.
- Hojas de cálculo.
- Navegación y edición web.
- etc.

## Distribuciones de Linux.
<<<<<<< HEAD

En el nucleo Linux incluye determinados programas para satisfacer las necesidades.

# Trying Out Commands

## who

```
~   my_dir  who
katherine console  May 23 20:43
katherine ttys000  Jun  4 11:45
katherine ttys001  Jun  4 12:16
```

## finger

```sh
~   my_dir  finger
Login    Name                 TTY  Idle  Login  Time   Office  Phone
katherine katherine            s00    10  Sat    11:45
katherine katherine            s00        Sat    12:16
katherine katherine           *con   11d  May 23 20:43
```

## whoami

```
~   my_dir  whoami
katherine
```

## hostname

```
~   my_dir hostname
RKMBP2014.local
```

## passwd

```
~   my_dir  passwd
Changing password for katherine.
Old Password:
New Password:
Retype New Password:

```

## exit

```
~   my_dir  exit
Saving session...completed.
Deleting expired sessions...      39 completed.

[Process completed]

```

## /

(Directorio raíz)

```
/
Applications System       Volumes      cores        etc          opt          sbin         usr
Library      Users        bin          dev          home         private      tmp          var
```

## /home

(Contiene los directorios de los usuarios)

## /bin

(Ordenes usuales y utilidades)

```
/bin
[         chmod     dash      df        expr      ksh       ln        mv        pwd       sh        sync      unlink
bash      cp        date      echo      hostname  launchctl ls        pax       rm        sleep     tcsh      wait4path
cat       csh       dd        ed        kill      link      mkdir     ps        rmdir     stty      test      zsh

```

## /usr

Programas, librerias y fícheros de uso normal

```
/usr
X11        X11R6      bin        lib        libexec    local      sbin       share      standalone
```

## /etc

Contiene ficheros de configuración.

```
/etc
afpovertcp.cfg                        gettytab~orig                         ntp_opendirectory.conf                rmtab
afpovertcp.cfg~orig                   group                                 openldap                              rpc


```

## /sbin

Contiene programas necesariosde inicio de sistema

```
/sbin
apfs_hfs_convert fsck             fstyp            kextload         mount_acfs       mount_fdesc      mount_tmpfs      newfs_msdos      ping6
apfs_unlockfv    fsck_apfs        fstyp_hfs        kextunload       mount_afp
```

## /tmp

Contiene ficheros temporales

```
/tmp
MozillaUpdateLock-2656FF1E876E9973 com.apple.launchd.RfLq2XEAyl       com.apple.launchd.sri8ZywjRR       powerlog
com.apple.launchd.EL6EmJ1P94       com.apple.launchd.V35areNMAj       com.google.Keystone
```

## /var

Contiene ficheros de spool de datos, logs...

```
/var
MobileSoftwareUpdate backups              empty                lib                  mail                 protected            rwho                 vm
agentx               chef                 folders              log                  msgs                 root                 select               yp
```

## /proc

Información sobre el sistema

## /lib

Librerias de ejecución

## pwd

Nos dice en cada momento la ruta completa de donde nos encontramos

```
~   ***pwd***
/Users/katherine
```

## ls

Nos muestra los archivos del directorio actual

```
~   labelfolders  **ls**
0_missing       0_no_expression 1_navy          2_skyblue       3_white         4_peachpuff     5_orangered
```

**ls fich**

```
12920340044 .               12920340045 0_no_expression 12920340048 4_peachpuff     12920340050 0_missing       12920340052 2_skyblue
12919956218 ..              12920340046 .DS_Store       12920340049 5_orangered     12920340051 1_navy          12920340053 3_white
```

**ls \*.html**

```
12920340044 .               12920340045 0_no_expression 12920340048 4_peachpuff     12920340050 0_missing       12920340052 2_skyblue
12919956218 ..              12920340046 .DS_Store       12920340049 5_orangered     12920340051 1_navy          12920340053 3_white
```

ls _imon_

```
cookbook  ls *imon*
pay-de-limon.html
```

**ls -l**

```
 ~  ls -l
total 0
drwx------@  3 katherine  staff    96 May 15 14:43 Applications
drwxr-xr-x   6 katherine  staff   192 Jun  4 12:00 Code
drwx------+  5 katherine  staff   160 Jun  2 10:35 Desktop
```

**ls -a**  
Muestra todos los ficheros (y también los ocultos que empiezan por .)

```
.                           .bash_history               .viminfo                    zsh_sessions               Documents                   Pictures
..                          .config                     .vscode                     szshrc                      Downloads                   Public
```

**ls -la**  
Muestra todos los archivos junto con su tamaño, usuario y grupo, fecha de modificación.

```
drwx------  33 katherine  staff   1056 Jun  4 11:53 .Trash
-rw-------   1 katherine  staff      4 May 31 17:49 .bash_history
drwxr-xr-x   4 katherine  staff    128 May 25 17:47 .config
-rw-r--r--   1 katherine  staff      0 May 20 10:35 .lesshsQ
```

**ls -d**
Muestra solo los directorios

**ls -R**
Muestra el directorio actual y los subdirectorios.

## mkdir

Crear directorios

## rmdir

Elimina directorios vacios

## cat

Muestra el contenido de un archivo

## head

Muestra las primeras 10 lineas de un archivo.

```
 nike-home  head nike.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="nike.css">
</head>
```

## tail

Muestra las ultimas 10 lineas de un archivo

```
nike-home  tail nike.css
    float: left;
    width: 80%;
    background: white;
}
aside {
    float: left;
    width: 20%;
    background: lightgreen;
```

## cp

Copiara los archivos y directorios.

```
Play  ls
copia1      directorio1
Play  cp copia1 ./directorio1
Play cd directorio1; ls
copia1
```

## mv

Movera archivos, carpetas o directorios al destino deseado. También cambia el nombre.

```
Play  mv copia1 archivo-1
Play  ls
archivo-1   directorio1
```

## rm -r

Elimina archivos, documentos y directorios.

```
Play  rm -r directorio1; ls
archivo-1
```

## .

Directorio actual.

## ..

Directorio padre.

```
~  ../
/Users
```

## ~

Directorio home.

```
Play  ~
~  pwd
/Users/katherine
```

## Simbolos especiales.

Actuan como comodines para uno o multiples caracteres.

```
ls *hou*
cats.jpg  home.css  home.html
```

**|**  
Pipe redirecciona la salida estándar,envia los datos de un comando a otro.

```
Code  ls | sort
exercises
github.com
scratc
```

**><**  
Trabajan con archivos intermedios.

```

```

## Variables del Shell

**echo $HOME**
Indica el directorio Home del usuario.

```
echo $HOME
/Users/katherine
```

**echo $PATH**
Directorios donde el sistema busca un comando.

```
echo $PATH
/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/Library/TeX/texbin:/opt/X11/bin
```

**echo $TERM**
Indica que tipo de terminal.

```
echo $TERM
xterm-256color
```

**echo $USER**
Nombre del usuario

```
echo $USER
katherine
```

**echo $UID**
Numero de identificación del usuario.

```
echo $UID
502
```

**echo $PS1**
Prompt del sistema

```
echo $PS1
%{$fg_bold[cyan]%}$ZSH_THEME_CLOUD_PREFIX %{$fg_bold[green]%} %{$fg[green]%}%c %{$fg_bold[cyan]%}$(git_prompt_info)%{$fg_bold[blue]%} % %{$reset_color%}
```
=======
En el nucleo Linux incluye determinados programas para satisfacer las necesidades
>>>>>>> 24887dfea822504e89334ad4bdb6fa67e1538849
