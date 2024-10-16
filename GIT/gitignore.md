## HOW TO CREATE GIT IGNORE
### Il git ignore è un file che possiamo includere nei nostri progetti e mi permetti di evitare di pushare sulla mia repository determinati file.
### Di solito, i file che vanno inseriti nel .gitignore sono quei file costruiti automaticamente dai pacchetti che installiamo, ad esempio:
    1. /node_modules o /packages
    2. compiled code, such as .o, .pyc, and .class files
    3. build output directories, such as /bin, /out, or /target
    4. files generated at runtime, such as .log, .lock, or .tmp
    5. hidden system files, such as .DS_Store or Thumbs.db
    6. personal IDE config files, such as .idea/workspace.xml

+ ```git **/logs ``` => tutte le dir chiamate *logs*