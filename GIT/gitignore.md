## HOW TO CREATE GIT IGNORE
### Il git ignore è un file che possiamo includere nei nostri progetti e mi permetti di evitare di pushare sulla mia repository determinati file.
### Di solito, i file che vanno inseriti nel .gitignore sono quei file costruiti automaticamente dai pacchetti che installiamo, ad esempio:
    1. /node_modules o /packages
    2. compiled code, such as .o, .pyc, and .class files
    3. build output directories, such as /bin, /out, or /target
    4. files generated at runtime, such as .log, .lock, or .tmp
    5. hidden system files, such as .DS_Store or Thumbs.db
    6. personal IDE config files, such as .idea/workspace.xml

+ ```**/logs ``` => tutte le dir chiamate *logs*

+ ```**/logs/debug.log ``` => tutti i file chiamati *debug* che hanno come parent una dir *logs*

+ ```*.logs ``` => tutti i file che si chiamano *qualcosa.logs*. L'asterisco è un carattere jolly corrisponde a uno o più caratteri

+ ```/debug.logs ``` => se viene anteposta una barra verranno ignorati tutti i file *debug.logs* nella dir principale

+ ```*debug.log``` => tutti i file *debug.log*

+ ```debug?.log ``` => tutti i file *debug1CHAR.log* (debug0.log, debugx.log). Il ? indica 1 character

+ ```debug[0-9].log ``` => tutti i file *debugNUMERO.log* (debug1.log , debug7.log)

+ ```debug[01].log ``` => tutti i file che hanno dopo *debug* uno dei caratteri numerici tra quadre (debug0.log , debug1.log )

+ ```debug[!01].log ``` => tutti i file che NON hanno dopo *debug* uno dei caratteri numerici tra quadre (debug2.log , debug3.log )

+ ```debug[a-z].log ``` => tutti i file che hanno dopo ***debug*** un carattere alfabetico (debuga.log)

+ ```Log ``` => tutti i file e le directory che hanno la parola *log*

+ ```logs/ ```=> tutte le **directory** che si chiamano logs

+ ```logs/**/debug.log ```=> tutte le dir logs con altre ***sottodir*** che contengono debug o solo debug (logs/debug , logs/dir/debug) 

+ ``` logs/*day/debug.log ``` => tutte le dir che si chiameranno ***logs/monday/debug***. Ovviamente anche thursday, wednesday etc

+ ``` logs/debug.log ``` => tutte le cartelle nella dir principale che si chiamano ***logs/*** e hanno un file ***debug***













