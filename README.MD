## PRÁCTICA GIT, MARKDOWN, GITHUB
## Identificación.
Andrés Sebastián Rodríguez Magallanes\
Lenguage de Marcas y Sistemas de Gestión.\
IES Aguadulce.\
1º Desarrollo de Aplicaciones Web.

## Uso de Git mediante la terminal git bash.
* Creación del repositorio en nuestro ordenador (_init_)

```
sebas@HP-Sebas MINGW64 /d/OneDrive/DAW/Lenguaje de Marcas/PracticaGit (master)
$ git init
Initialized empty Git repository in D:/OneDrive/DAW/Lenguaje de Marcas/PracticaGit/.git/
```
* Creación de un commit inicial (_add_, _status_, _commit_, _log_),
```
sebas@HP-Sebas MINGW64 /d/OneDrive/DAW/Lenguaje de Marcas/PracticaGit (master)
$ git add index.html README.MD
```
```
sebas@HP-Sebas MINGW64 /d/OneDrive/DAW/Lenguaje de Marcas/PracticaGit (master)
$ git commit -m "Creamos archivo index.html y readme.md "
[master (root-commit) ce094f9] Creamos archivo index.html y readme.md
 2 files changed, 61 insertions(+)
 create mode 100644 README.MD
 create mode 100644 index.html
```
```
sebas@HP-Sebas MINGW64 /d/OneDrive/DAW/Lenguaje de Marcas/PracticaGit (master)
$ git log
commit ce094f9f371654cbd033a05ef931d4eee8520cb4 (HEAD -> master)
Author: Sebastian <sebas517@hotmail.com>
Date:   Mon Jan 15 21:22:29 2024 +0100

    Creamos archivo index.html y readme.md
```
* Creación del repositorio en _Github_

![Crear repositorio en Github](/Capturas/cap01.jpg)

* Añadir el remoto al repositorio local (_branch_, _remote_)

```
sebas@HP-Sebas MINGW64 /d/OneDrive/DAW/Lenguaje de Marcas/PracticaGit (master)
$ git branch
* master
```
```
sebas@HP-Sebas MINGW64 /d/OneDrive/DAW/Lenguaje de Marcas/PracticaGit (master)
$ git remote add origin https://github.com/SebasRodMag/PracticaGit.git
```
```
sebas@HP-Sebas MINGW64 /d/OneDrive/DAW/Lenguaje de Marcas/PracticaGit (master)
$ git remote -v
origin  https://github.com/SebasRodMag/PracticaGit.git (fetch)
origin  https://github.com/SebasRodMag/PracticaGit.git (push)
```
* Subir el repositorio a Github (_push_)

```
sebas@HP-Sebas MINGW64 /d/OneDrive/DAW/Lenguaje de Marcas/PracticaGit (master)
$ git push origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 1016 bytes | 338.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/SebasRodMag/PracticaGit/pull/new/master
remote:
To https://github.com/SebasRodMag/PracticaGit.git
 * [new branch]      master -> master
```
* Comprobar que está subido a Github.

![Vista repositorio](/Capturas/cap02.jpg)