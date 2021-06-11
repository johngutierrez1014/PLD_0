**README**
Is software for tracking changes in any set of files, usually used for coordinating work among programmers collaboratively developing source code during software development. Its goals include speed, data integrity, and support for distributed, non-linear workflows (thousands of parallel branches running on different systems).
| Tipo | Description | Command |
|--|--|--|
| **Git clone** | Git clone is a command to download the existing source code from a remote repository | git clone `<URL>`|
| **Git branch** | Branches are highly important in the world of Git. Using branches, multiple developers can work in parallel on the same project simultaneously. | git branch `<nombre-de-la-rama>` |
|| Visualización de ramas: | git branch | 
|| | git branch --list |
|| Borrar una rama: | git branch -b `<nombre-de-la-rama>`|
| Git checkout | This is also one of the most used commands in Git. To work on a branch, you first have to switch to it. We will use git checkout mainly to switch you from one branch to another. We can also use it to check files and commits. | git checkout `<nombre-de-la-rama>` |
| **Git status** | El comando de git status nos da toda la información necesaria sobre la rama actual. | git status |
| **Git add** | Cuando creamos, modificamos o eliminamos un archivo, estos cambios suceden en local y no se incluirán en el siguiente commit (a menos que cambiemos la configuración). | git add `<archivo>` |
|| Añadir todo de una vez: | git add -A |
| **Git commit** | Git commit es como establecer un punto de control en el proceso de desarrollo al cual puedes volver más tarde si es necesario. | git commit -m "mensaje de confirmación" |
| **Git push** | Después de haber confirmado tus cambios, el siguiente paso que quieres dar es enviar tus cambios al servidor remoto. Git push envía tus commits al repositorio remoto. | git push <nombre-remoto> <nombre-de-tu-rama> |
|||git push -u origin <nombre-de-tu-rama>|
|**Git pull** | El comando git pull se utiliza para recibir actualizaciones del repositorio remoto. Este comando es una combinación del git fetch y del git merge lo cual significa que cundo usemos el git pull recogeremos actualizaciones del repositorio remoto (git fetch) e inmediatamente aplicamos estos últimos cambios en local (git merge). | git pull <nombre-remoto> |
| **Git revert** | A veces, necesitaremos deshacer los cambios que hemos hecho. Hay varias maneras para deshacer nuestros cambios en local y/o en remoto (dependiendo de lo que necesitemos), pero necesitaremos utilizar cuidadosamente estos comandos para evitar borrados no deseados. | git revert 3321844 |
