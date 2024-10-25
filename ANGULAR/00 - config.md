# CONFIGURAZIONE PRIMO PROGETTO ANGULAR

### Installazione globale
```bash
npm install -g @angular/cli 
``` 

### HELP 
```bash
ng --help 
ng new --help    <!-- Aiuto su specifico comando -->
``` 

## CREATE, BUILD AND SERVE

### Init di un nuovo progetto + install node modules
```bash
ng new nome_progetto
N - scelta del tipo di css - N
``` 

### use 
```bash
cd my-first-project
``` 

### run project
```bash
ng serve
``` 

### build project - creazione di una build per la distribuzione del progetto
```bash
ng build *nomeProgetto* || ng b *nomeProgetto*
```

### create component
```bash
ng generate component test/test  <!-- in questo modo genera una cartella test con un component test all'interno -->
```

### create class
```bash
ng generate class models/persona 
```

### create service
```bash
ng generate service services/prodotto   
```
// (lo chiamerà prodotto.service)
