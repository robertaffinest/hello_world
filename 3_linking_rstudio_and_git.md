Ecco una guida per l'utente su come collegare Git/GitHub e RStudio e gestire il controllo delle versioni:

---

## Guida all'uso di Git/GitHub con RStudio

### Introduzione
Questa guida ti guiderà attraverso i passaggi per collegare Git e GitHub a RStudio, così da poter gestire il controllo delle versioni del tuo codice direttamente dall'ambiente RStudio.

### 1. Collegare Git e RStudio

1. **Apri RStudio**:
   - Avvia RStudio sul tuo computer.

2. **Accedi alle Opzioni Globali**:
   - Vai su *Tools > Global Options*.

3. **Configura Git**:
   - Seleziona la scheda *Git/SVN*.
   - Assicurati che la casella per l'uso di Git come sistema di controllo versioni sia selezionata.
   - Verifica il percorso dell'eseguibile Git (git.exe). Se il percorso è errato, correggilo nel campo specifico.
   - Clicca su *OK* o *Apply* per salvare le modifiche.

### 2. Collegare RStudio e GitHub

1. **Genera una Chiave RSA**:
   - Nella stessa finestra di opzioni (Git/SVN), clicca su *Create RSA Key* e poi su *Close* quando il processo è completato.

2. **Copia la Chiave Pubblica**:
   - Clicca su *View public key*, copia la chiave pubblica che appare e chiudi la finestra.

3. **Aggiungi la Chiave a GitHub**:
   - Vai su [GitHub](https://github.com) e accedi al tuo account.
   - Vai su *Settings* (Impostazioni), poi su *SSH and GPG keys* e clicca su *New SSH key*.
   - Incolla la chiave pubblica nel campo *Key* e dai un titolo alla chiave (es. "Chiave RStudio").
   - Conferma l'aggiunta inserendo la tua password di GitHub.

### 3. Creare un Nuovo Repository su GitHub

1. **Crea un Repository**:
   - Vai su [GitHub](https://github.com), accedi al tuo profilo e seleziona *Repositories*.
   - Clicca su *New* e compila il modulo per creare un nuovo repository (dai un nome e una breve descrizione).
   - Clicca su *Create repository* e copia l'URL del repository appena creato.

### 4. Creare un Progetto in RStudio

1. **Crea un Nuovo Progetto**:
   - In RStudio, vai su *File > New Project*.
   - Seleziona *Version Control* e poi *Git*.
   - Incolla l'URL del repository che hai copiato precedentemente.
   - Scegli la directory dove desideri salvare il progetto e clicca su *Create Project*.

### 5. Scrivere e Salvare un File R

1. **Crea uno Script R**:
   - Vai su *File > New File > R Script*.
   - Inserisci il seguente codice:
     ```r
     print("This file was created within RStudio")
     print("And now it lives on GitHub")
     ```
   - Salva il file nella directory del progetto.

### 6. Staging, Commit e Push del File

1. **Gestisci i File in Git**:
   - Nella scheda *Git* nel quadrante dell'ambiente di RStudio, dovresti vedere il file appena creato.
   - Seleziona la casella sotto *Staged* per preparare il file al commit.

2. **Effettua il Commit**:
   - Clicca su *Commit*. Nella finestra che si apre, inserisci un messaggio di commit e clicca su *Commit* per salvare le modifiche.

3. **Esegui il Push**:
   - Dopo il commit, clicca su *Push* per inviare le modifiche al tuo repository GitHub.

### 7. Verifica il Commit su GitHub

1. **Controlla il Repository**:
   - Vai su GitHub e accedi al tuo repository per vedere il commit che hai appena inviato.

### Riepilogo
Hai ora collegato con successo Git e RStudio, generato e aggiunto una chiave SSH a GitHub, creato un nuovo repository, e gestito i file di progetto con Git tramite RStudio.

Per ulteriori informazioni e supporto, consulta la documentazione ufficiale di RStudio e GitHub.

---

Se hai altre domande o hai bisogno di ulteriori chiarimenti, fammi sapere!
