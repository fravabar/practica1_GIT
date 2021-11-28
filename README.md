# practica1_GIT
Practica 1: Curso de git, gitHub y Sourcetree

- ¿Qué comando utilizaste en el paso 11? ¿Por qué? 

git reset --hard HEAD~1

git reset HEAD~1 deshace el último copy, además utilizamos --hard ya que queremos deshacer los cambios en Working copy 

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? 

1º git reflog para averiguar el log del commit eliminado(sin utilizar)
2ª git reset --hard <log del commit> para rehacer el commit y devolver los cambios al archivo en el Working copy

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué? 

No, ya que el commit realizado en styled tendría acceso directo al del master en la secuencia de commits

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 

Si,  causa conflicto ya que no podemos acceder de manera directa desde la rama styled a la rama htmlify en el grafo y además el archivo git-nuestro.md es diferente en las 2 ramas.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 

No, al poderse acceder al último commit en styled desde el último de master en la misma linea del grafo, el puntero de master avanza hasta el del styled (Fast-forward)

- ¿Qué comando o comandos utilizaste en el paso 25? 

git log --graph --pretty=oneline

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 

Es Fast-forward ya que nos esta avanzando  la posición del HEAD del Commit 4 donde se encuentra master en el grafo al Commit 5 creado por htmlify.

- ¿Qué comando o comandos utilizaste en el paso 27? 

git reset HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28? 

git restore git-nuestro.md

- ¿Qué comando o comandos utilizaste en el paso 29? 

git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30? 

git branch title
git checkout title
git reset --hard <id del log>
git checkout master
git merge title

- ¿Qué comando o comandos usaste en el paso 32? 

git log
git reset --hard <id del commit>

- ¿Qué comando o comandos usaste en el punto 33? 

git reflog
git reset --hard <id del log>
