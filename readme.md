- ¿Qué comando utilizaste en el paso 11? git reset --hard HEAD~1 
¿Por qué? con él comando reset puedo mover la rama hasta el commit que quiera, en este caso me vale hacer un HEAD~1 que le indica que deshaga el commit anterior. Le añado el parámetro --hard para que me deje el working copy como estaba a la hora de hacer el primer commit. Por otro lado también me podia haber situado directamente en el commit correspondiente usando su identificador (con git log y despues un git reset al commit que me interese). 

- ¿Qué comando o comandos utilizaste en el paso 12? git reflog y git reset --hard abe67bf
¿Por qué? con git reflog busco el commit que me interesa y selecciono su id, después me situo en él con reset. 

- El merge del paso 13, ¿Causó algún conflicto? No ¿Por qué? Porque la rama styled contiene todos los commit's de master, es su padre.

- El merge del paso 19, ¿Causó algún conflicto? Sí, ¿Por qué? Porque la rama styled necesita absorver los commit's de htmlify y tiene un commit donde se modifica un fichero común. 

- El merge del paso 21, ¿Causó algún conflicto? No ¿Por qué? Porque la rama styled tenía absorvidos todos los cambios, tan sólo se ha puesto el puntero de master apuntando al mismo commit que styled. (Fast Forward)

- ¿Qué comando o comandos utilizaste en el paso 25?
git log --graph --decorate --all

- El merge del paso 26, ¿Podría ser fast forward? Sí ¿Por qué? Porque la rama title es la única hija de master. 

- ¿Qué comando o comandos utilizaste en el paso 27? git reset HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28? git checkout -- git-nuestro.md

- ¿Qué comando o comandos utilizaste en el paso 29?  git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30? git reflog y despues git reset --hard eaf8919.

- ¿Qué comando o comandos usaste en el paso 32? git reflog y git reset --hard fe37d3b (al primer commit)

- ¿Qué comando o comandos usaste en el punto 33? git reflog y git reset eaf8919