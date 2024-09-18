
# Guida Utente: Gestione dei Progetti in RStudio con Git e GitHub

## 1. Collegamento di un Progetto Esistente a Git

### Creazione di un Progetto R senza Controllo Versione

1. **Apri RStudio**.
2. Vai su **File** > **New Project** > **New Directory** > **New Project**.
3. Dai un nome al tuo progetto.
4. **Non** selezionare l'opzione **"Create a git repository"**.
5. Clicca su **Create Project**.

### Inizializzazione di Git

1. **Apri Git Bash** (o il Terminale).
2. Naviga nella directory del tuo progetto utilizzando il comando:
   ```bash
   cd ~/dir/name/of/path/to/file
   ```
   Assicurati che il prompt mostri il percorso corretto della tua directory.
3. Inizializza il repository Git locale con il comando:
   ```bash
   git init
   ```
4. Aggiungi tutti i file del progetto al repository:
   ```bash
   git add .
   ```
5. Commetti le modifiche con un messaggio descrittivo:
   ```bash
   git commit -m "Initial commit"
   ```

## 2. Collegamento del Progetto a GitHub

### Creazione di un Repository su GitHub

1. Vai su [GitHub.com](https://github.com) e accedi al tuo account.
2. Crea un nuovo repository:
   - Assicurati che il nome del repository corrisponda esattamente al nome del tuo progetto R.
   - **Non** inizializzare il repository con un README, un .gitignore o una licenza.

### Collegamento del Repository Locale a GitHub

1. Dopo aver creato il repository su GitHub, troverai una sezione con istruzioni per **"Push an existing repository from the command line"**.
2. Copia e incolla i comandi forniti da GitHub nel terminale:
   ```bash
   git remote add origin <URL-del-tuo-repository>
   git branch -M main
   git push -u origin main
   ```
3. Dopo aver eseguito questi comandi, aggiorna la pagina del tuo repository su GitHub. Dovresti vedere i tuoi file del progetto.

4. **Riavvia RStudio** e apri il tuo progetto. Ora dovresti vedere la scheda **Git** nell'angolo in alto a destra, che ti permetterà di gestire il versionamento e di spingere le modifiche su GitHub direttamente da RStudio.

## 3. Lavorare con un Repository GitHub Esistente

### Clonazione di un Repository Esistente

1. In RStudio, vai su **File** > **New Project** > **Version Control**.
2. Seleziona **Git** come sistema di controllo versione.
3. Inserisci l'URL del repository GitHub che desideri clonare.
4. Scegli una posizione sul tuo computer per memorizzare i file localmente.
5. Clicca su **Create Project**.

### Gestione del Repository Clonato

1. Tutti i file esistenti del repository saranno ora memorizzati localmente sul tuo computer.
2. Puoi modificare i file e spingere le modifiche su GitHub direttamente dall'interfaccia di RStudio.

## Riassunto

In questa guida, hai imparato a:

- Convertire un progetto R esistente per utilizzare il controllo versione con Git.
- Collegare un progetto Git a GitHub.
- Clonare un repository GitHub esistente e lavorare su di esso in RStudio.

Con questi passaggi, sarai in grado di gestire efficacemente il controllo versione e collaborare su progetti utilizzando Git e GitHub.

---

Spero che questa guida sia chiara e utile! Se hai altre domande o hai bisogno di ulteriori dettagli, fammelo sapere.
