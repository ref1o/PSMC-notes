# Guida all'Importazione di una Repo Obsidian da GitHub

Per importare una repository Obsidian da GitHub sul tuo computer, segui questi passaggi:

1. **Clona la Repository**:
   - Assicurati di avere [Git](https://git-scm.com/) installato sul tuo computer. Se non l'hai già fatto, puoi scaricarlo da [qui](https://git-scm.com/downloads).
   - Apri il tuo terminale o prompt dei comandi.
   - Naviga nella cartella in cui desideri clonare la tua repo Obsidian utilizzando il comando `cd` (cambia directory) e poi esegui il seguente comando:
     ```bash
     git clone <URL-della-repository>
     ```
     Assicurati di sostituire `<URL-della-repository>` con l'URL effettivo della tua repository Obsidian su GitHub.

2. **Configura Obsidian**:
   - Apri l'applicazione Obsidian sul tuo computer.

3. **Apri la Cartella della Repo**:
   - Una volta aperto Obsidian, vai su "Impostazioni" (nell'angolo in alto a destra).
   - Nella sezione "Altre", trova l'opzione "Apri cartella della nota" e clicca su "Apri".
   - Naviga nella cartella che hai clonato dalla repository GitHub e selezionala.

4. **Carica le Tua Note**:
   - Ora che hai aperto la cartella della repo Obsidian in Obsidian stesso, puoi vedere e modificare le tue note.

5. **Sincronizza con GitHub** (opzionale):
   - Se desideri sincronizzare le tue modifiche con GitHub, dovrai farlo manualmente utilizzando Git. Per eseguire il commit e il push delle modifiche, segui questi passaggi:
     ```bash
     # Aggiungi i tuoi cambiamenti
     git add .

     # Esegui il commit con un messaggio
     git commit -m "Aggiornamenti alle note"

     # Effettua il push dei tuoi cambiamenti su GitHub
     git push origin master
     ```
