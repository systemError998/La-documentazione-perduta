# GIT REVERT
Talvolta dobbiamo annullare modifiche che abbiamo effettuato. 
Ci sono vari modi per annullare le modifiche, sia localmente che su remoto (a seconda delle necessità), ma dobbiamo essere cauti con questi comandi per evitare cancellazioni indesiderate.

###### Per vedere la nostra cronologia di commit
```git log --oneline```

###### Poi dobbiamo solo specificare il codice hash vicino al commit che vorremmo annullare:
Il comando git revert annullerà il commit specificato creando un nuovo commit senza eliminare quello vecchio.
```git revert 3321844```

Il vantaggio dell'uso di git revert è che non tocca la cronologia dei commit. 
Questo significa che puoi ancora vedere tutti i commit nella tua cronologia, anche quelli ripristinati.

Un'altra misura di sicurezza qui è che tutto accade localmente a meno che non inviamo (**git push**) i commit al repository remoto.