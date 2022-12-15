# DCA: Práctica 9.
## David Bernabeu Ferrer

Para el alias local: git config --local alias.lg "log --oneline --decorate --graph"
Para el alias global: git config --global alias.st "status"


Hacemos variso commits, introducimos fallo,
hacemos mas commits.
$ git bisect start
$ git bisect good 7c8b38e
$ git bisect bad 6b0c0e9
$ git bisect bad
$ git bisect bad

C:\Users\david\Documents\Universidad\DCA\Practica\Practica9>git bisect bad 6b0c0e9
Bisecting: 1 revision left to test after this (roughly 1 step)
[7a9803a0866d8db7a5d0afc7742e48f33e9e4b70] Seguimos desarrollando...

C:\Users\david\Documents\Universidad\DCA\Practica\Practica9>git status
HEAD detached at 7a9803a
You are currently bisecting, started from branch 'master'.
  (use "git bisect reset" to get back to the original branch)

nothing to commit, working tree clean

C:\Users\david\Documents\Universidad\DCA\Practica\Practica9>git bisect bad

0f3c2fcafccba3248d0dec1bf9a77242bd474139 is the first bad commit
commit 0f3c2fcafccba3248d0dec1bf9a77242bd474139
Author: David Bernabeu Ferrer <71643167+dvddepennde@users.noreply.github.com>
Date:   Thu Dec 15 16:46:35 2022 +0100

    Añadimos fallo

 hola.py | 6 +++---
 1 file changed, 3 insertions(+), 3 deletions(-)


 ## Hooks
 Uso del pre-commit
 ![](./foto.png)