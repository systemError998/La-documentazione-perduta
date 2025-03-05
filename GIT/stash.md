# STASH

## Intro
L'area di **stash** è un'area di **accantonamento** dove poter conservare **TEMPORANEAMENTE** i cambiamenti senza inviarli alla repo.
Questa funzionalità è utile quando hai fatto modifiche in un branch, ma **_non sei ancora pronto per passarle alla fase di commit, tuttavia vorresti passare a un altro branch._**

###### Salvare modifiche nello stash
Questo salva le modifiche e riporta la directory di lavoro allo stato nella quale si trovava all'ultimo commit. Le modifiche accantonate nello stash sono disponibili per qualsiasi branch in quel repository.

```git stash save "messaggio opzionale"```

NB _le modifiche che vuoi accantonare nello stash devono essere su file tracciati. Se hai creato un nuovo file e cerchi di accantonare le tue modifiche, potresti ottenere l'errore No local changes to save_

###### Visualizzare modifiche nello stash
Questo comando restituisce un elenco delle tue istantanee salvate

```git stash list```

###### Recuperare modifiche nello stash

Applica le modifiche e lascia una copia nell'area di stash
```git stash apply NOME-STASH  ```

Applica le modifiche e rimuove i file dall'area di stash
```git stash pop NOME-STASH```

##### Eliminare le Modifiche nello Stash

Eliminare le modifiche accantonate senza applicarle esegui il comando:
```git stash drop NOME-STASH```

Per eliminare l'intera area di stash
```git stash clear```
