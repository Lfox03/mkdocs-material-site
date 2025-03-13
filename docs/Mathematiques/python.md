---
title: Example de code python 
description: Introduction aux codes python les plus communs dans les éxercices de mathématiques.
---
## Les boucles

Les boucles permettent de répéter un code. Chaque exécution de la boucle est appelé une **itération**

En python, il existe deux types de boucle:

=== "Boucle For"

    La boucle ```for``` (en français **"Pour"**) est une boucle qui est exécutée pour un nombre déterminé d'itérations

    Voici un example :

    ``` py title="Boucle 'for'" linenums="1"
    nombre = 0
    for i in range (0, 10):
        nombre = nombre + 1
    print(nombre)
    ```

    Elle incrémente la variable ```nombre``` tant que ```i``` est entre 0 et 10.

=== "Boucle While"

    La boucle ```while``` (en français **"tant que"**) est une boucle qui est exécutée tant qu'une certaine condition est valide.

    ``` py title="Boucle 'while'" linenums="1"
    nombre = 0
    while nombre < 10:
        nombre = nombre + 1
    print(nombre)
    ``` 

    !!! warning "attention aux boucles infinies !"
        Veillez à ce que la condition d'arrêt de la boucle soit atteint, autrement elle deviendra une **boucle infini** !


voila quoi, sinon voici des maths lol:

$$
\cos x=\sum_{k=0}^{\infty}\frac{(-1)^k}{(2k)!}x^{2k}
$$