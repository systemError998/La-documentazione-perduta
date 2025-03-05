# ISTRUZIONI GIT FOR BRANCHING
```git branch``` => check su quale branch sono
```git branch nomeBranch``` => creo un nuovo branch
```git checkout nomeBranch``` => mi sposto su un altro branch
``` branch -d nomeBranch``` => elimina il branch

Per inviare il nuovo branch al repository remoto, devi usare questo comando:
```git push -u <remoto> <nome-branch>```

```git branch --list```

elimina branch morti
```git fetch --all --prune```

creare e portarsi su un branch allo stesso tempo: crea un nuovo branch localmente (-b sta per branch) quindi passa ad esso non appena viene creato.
```git checkout -b <nome-del-tuo-nuovo-branch>```



Il merge va fatto sempre dal branch master  
Prima portati nel branch dev:

```git checkout dev```
Prima dell'integrazione, dovresti aggiornare il tuo branch dev locale:

```git fetch```
Alla fine, puoi integrare il tuo branch nel branch dev:

```git merge <nome-branch>```