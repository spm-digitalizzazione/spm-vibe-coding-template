# SPM - Vibe Coding Starter Template

Benvenuto nel repository template ufficiale per le applicazioni **Vibe-Coded** create con **Lovable** (o piattaforme AI affini) all'interno di **SPM S.p.A.**.

Questo repository costituisce il punto di partenza **obbligatorio** per ogni nuovo progetto sviluppato da personale non tecnico o da team interni.

---

## 🎯 A cosa serve questo Template?

Il template è stato progettato dalla Direzione Tech per consentire a chiunque in azienda di prototipare e creare applicativi in autonomia, garantendo al contempo la sicurezza dei dati aziendali e la conformità ai criteri di cybersecurity.

Il repository include già preconfigurati:

- **`.gitignore`**: Un filtro avanzato che impedisce il caricamento accidentale su GitHub di dati sensibili (fogli Excel, CSV, PDF, credenziali, file `.env`).
- **`AGENTS.md`**: Il file di regole e vincoli architetturali che l'AI di Lovable legge ed applica automaticamente durante la generazione del codice (es. elaborazione dati esclusivamente _Client-Side_).
- **`SECURITY.md`**: La policy di sicurezza per chi sviluppa con questo template (dove possono stare i dati, cosa fare in caso di incidente, come segnalare una vulnerabilità).

---

## 🚀 Come utilizzare questo Template (Passo-Passo)

1. **Crea il tuo Repository:**
   - Clicca sul pulsante verde **"Use this template"** in alto a destra e seleziona **"Create a new repository"**.
   - Assegna un nome chiaro al tuo progetto (es. `gestione-turni-stampaggio`).
   - **IMPORTANTE:** Imposta la visibilità del repository su **Private**.
2. **Aggiungi l'Account di Supervisione (Obbligatorio):**
   - Vai nelle **Settings** del tuo nuovo repository -> **Collaborators** -> **Add people**.
   - Cerca e aggiungi l'indirizzo e-mail: `digitalizzazione@spmspa.it`.
3. **Collega Lovable:**
   - Accedi a Lovable con il tuo account aziendale (**Google SSO**).
   - Seleziona **"Import from GitHub"** e scegli il repository appena creato per iniziare a sviluppare.

---

## ⚠️ Gestione delle Regole e Responsabilità

### Modifica del file `.gitignore`

Il file `.gitignore` blocca di default tutti i tipi di file che potrebbero contenere informazioni riservate.

- È possibile aggiungere eccezioni per includere specifici file non sensibili (es. file di test) seguendo le istruzioni contenute in cima al file `.gitignore` stesso.
- **Le eccezioni devono essere aggiunte con estrema parsimonia e solo se strettamente necessarie.**

> 🚨 **NOTA SULLA RESPONSABILITÀ**
> La modifica o la rimozione delle regole di sicurezza presenti in questo template (`.gitignore`, `AGENTS.md` e `SECURITY.md`) **comporta l'assunzione diretta di responsabilità** da parte dell'utente in merito a eventuali fughe di dati (Data Leak), caricamenti di file riservati o violazioni delle policy informatiche aziendali.

---

## 📬 Supporto e Contatti

Per qualsiasi dubbio operativo, assistenza nell'impostazione dei progetti, o per richiedere la pubblicazione/condivisione di un'applicazione con altri colleghi, contatta il team di riferimento:

📧 **E-mail di Supporto:** `digitalizzazione@spmspa.it`
