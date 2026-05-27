# Documentacion del conflicto de fusion resuelto

## Descripcion del conflicto

Durante el desarrollo del proyecto, dos integrantes del equipo editaron
el mismo archivo en ramas diferentes, lo que genero un conflicto de fusion.

## Archivos en conflicto

- notebooks/proyecto_titanic.ipynb
- data/README.md

## Como ocurrio

Jacobo edito el archivo README.md en la rama/analisis-estadistico-inicial
y Helen edito el mismo archivo en la rama/unificacion-datos con contenido
diferente. Al intentar hacer el merge de las ramas a main, Git detecto
que ambas ramas habian modificado los mismos archivos.

## Como se resolvio

El conflicto se resolvio desde la Terminal usando los siguientes comandos:

git checkout --ours notebooks/proyecto_titanic.ipynb
git add notebooks/proyecto_titanic.ipynb
git commit -m "Resolver conflicto de fusion"
git push

Se decidio mantener la version de cada integrante en su respectivo merge.