# Git Tutorial



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
dove ```path/to/``` rappresenta il percorso della cartella ```VerificaDambra```.

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

```git init  # Inizializza il repository locale```
```git add README.md  # Inserimento del file README.md nell'area di staging```
```git commit -m "first commit"  # Creazione del primo commit, che serve a sincronizzare il repository locale con lo stage```
```git branch -M main  # Creazione del branch main, da usare come default```
```git remote add origin https://github.com/<username>/Esercitazione16maggio  # Connessione del repository remoto al repository locale```
```git push -u origin main  # Sincronizzazione del repository remoto con quello locale```


Nel caso in cui appaia questa finestra

<img width="286" alt="credential" src="https://github.com/ilREE/TutorialHelp/assets/129156247/9ac89568-3d97-435a-b2a3-d512d41ebe92">

selezionare ```manager-ui.```


Nel caso, invece, in cui il comando push non dovesse andare a buon fine a causa di problemi con
l'autenticazione, è stato configurato un account globale, pertanto bisogna eseguire questi passi:

- aprire il seguente link https://github.com/settings/tokens
- generare un token mediante ```Generate new token (classic)```
- confermare l'accesso inserendo la propria password, se richiesto
- in ```Note``` inserire un messaggio come "token di accesso"
- ```Expiration```: "No expiration"
- In ```Select scopes``` spuntare la casella accanto a ```repo```, in modo tale da avere la situazione sottostante
- generare il token e salvarlo in un file di testo





![token](https://github.com/ilREE/TutorialHelp/assets/129156247/b4f7b350-c07d-4567-acf9-436fbfc2a335)



Dopodiché, eseguire nuovamente il comando push usando il seguente formato:

```git push https://<username>:<token>@github.com/<username>/<reponame>.git```
dove ```<username>``` è il vostro username, al posto di ```<token>``` bisogna inserire il token creato prima e ```<reponame>``` è il nome del repository sul quale si vuole effettuare il ```push``` (in questo caso, ```<reponame>``` è ```Git-tutorial).```



# Aggiunta di nuovi file al repository

1. Creare un nuovo file main.c nel workspace
2. Implementare un programma che, dati in input 10 numeri positivi, trovi il massimo e lo visualizzi a video
3. Aggiungere il nuovo file nell'area di staging
4. Sincronizzare l'area di staging con il repository locale (usando un messaggio di commit congruo)
5. Sincronizzare il repository remoto con quello locale

Per ognuno dei punti, effettuare, separatamente, i punti da 2 a 5 per sincronizzare i repository.

Di seguito vi sono delle istruzioni per migliorare la formattazione del file README.md

# NOTA: Il repository che creerete in questa esercitazione vi sarà utile per le prossime esercitazioni.

# Migioramento del file README.md

- Aggiungere la traccia dell'esercizio svolto
- Aggiungere una descrizione del codice
- Inserire una sezione in cui vengono spiegati i comandi utilizzati per la creazione di questo repository in stile tutorial
- Spiegare, in una nuova sezione, le funzioni base di Git


# Inserire immagini nel README.md
Aggiungere l'immagine img.jpg al progetto ed inserirla nel testo con il seguente comando: ![](nome dell'immagine.png/img)


# Inserire sezioni
Le sezioni possono essere create inserendo un # prima del titolo della sezione. Si può modificare il tipo di sezione usando da uno a sei #. È importante separare i # dal titolo con uno spazio.

# Inserire codice e citazioni
Il codice può essere inserito delimitandolo con tre backtick `.

Le citazioni possono essere fatte aggiungendo > prima del testo.
