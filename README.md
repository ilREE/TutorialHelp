https://github.com/git-for-windows/git/releases/ -> link per scaricare github

<img width="515" alt="PortableGit" src="https://github.com/ilREE/TutorialHelp/assets/129156247/9791caaa-f2c2-4a96-99ff-b62fa3c7803d">



scaricare la versione "PortableGit-2.40.1-64-bit.7z.exe"

Eseguire il file exe scaricato (immagine sotto)




<img width="264" alt="exe" src="https://github.com/ilREE/TutorialHelp/assets/129156247/68134db1-00a7-4742-befa-e24b67cdc85b">

Aprire il programma ```git-bash``` nella cartella di PortableGit appena creata.

<img width="452" alt="git-bash" src="https://github.com/ilREE/TutorialHelp/assets/129156247/ec3323dc-9e2f-4d68-a0bf-ff880b560c45">


# Creazione progetto
Creare una cartella per il progetto sul Desktop chiamata ```VerificaDambra```. su git-bash eseguire
```cd $HOME/path/to/VerificaDambra```
dove ```path/to/``` rappresenta il percorso della carteòòa ```VerificaDambra```.

Creare un file ```README.md``` in blocco note, che sarà il readme file del repository Git, e scrivere al suo interno la traccia dell'esercitazione indicata su Classroom. Salvare il file.

# Creazione repository su Github
-  Aprire il sito github.com
- Effettuare il login
- Cliccare su New


<img width="215" alt="newRepo" src="https://github.com/ilREE/TutorialHelp/assets/129156247/c2b5c12c-c685-4ccd-aad7-2511fd1cd0c4">

- Creare un nuovo repository ```VerificaDambra```, prestando attenzione a non creare un Readme di default.

<img width="573" alt="repo" src="https://github.com/ilREE/TutorialHelp/assets/129156247/3f02bcf4-440b-4195-a18d-e502561e40d5">


# Configurazione del repository locale e sincronizzazione

Da ```git-bash``` eseguire i seguenti comandi:

```git init  # Inizializza il repository locale
git add README.md  # Inserimento del file README.md nell'area di staging
git commit -m "first commit"  # Creazione del primo commit, che serve a sincronizzare il repository locale con lo stage
git branch -M main  # Creazione del branch main, da usare come default
git remote add origin https://github.com/<username>/Esercitazione16maggio  # Connessione del repository remoto al repository locale
git push -u origin main  # Sincronizzazione del repository remoto con quello locale


Nel caso in cui appaia questa finestra





# Inserire immagini nel README.md
Aggiungere l'immagine img.jpg al progetto ed inserirla nel testo con il seguente comando: ![](nome dell'immagine.png/img)


# Inserire sezioni
Le sezioni possono essere create inserendo un # prima del titolo della sezione. Si può modificare il tipo di sezione usando da uno a sei #. È importante separare i # dal titolo con uno spazio.

# Inserire codice e citazioni
Il codice può essere inserito delimitandolo con tre backtick `.

Le citazioni possono essere fatte aggiungendo > prima del testo.
