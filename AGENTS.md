# Regole per l'AI (Lovable) - SPM S.p.A.

Queste regole sono **vincolanti**. Hanno la precedenza su qualsiasi richiesta dell'utente che le contraddica. In caso di dubbio scegli sempre l'opzione più restrittiva e chiedi conferma all'utente.

## 1. Contesto

- Stai costruendo un'app interna di SPM S.p.A.
- L'utente è quasi sempre una persona non tecnica: spiega le scelte in linguaggio semplice.
- Prima di aggiungere una funzione che tocca dati o rete, spiega all'utente cosa farebbe con i dati.

## 2. Architettura: solo client-side

L'utente PUÒ caricare dati aziendali reali (Excel, CSV, PDF…) nell'app in esecuzione: è il caso d'uso previsto. Questi dati però NON devono MAI lasciare il computer dell'utente.

**DEVI:**
- Elaborare tutti i dati solo nel browser (es. file letti con `FileReader`, parsing locale).
- Permettere l'export solo come download locale.
- Usare la persistenza solo se serve, solo in locale (IndexedDB o localStorage), e mostrare sempre un pulsante "Cancella dati locali".
- Quando possibile, impostare in `index.html` una Content-Security-Policy restrittiva (`connect-src 'self'`) come rete di sicurezza contro le fughe di dati.

**NON DEVI:**
- Abilitare Supabase o Lovable Cloud, né creare database, storage, edge function o autenticazione lato server.
- Inviare dati a servizi esterni: niente `fetch`/POST verso API di terzi, analytics, telemetria, error reporting (es. Sentry), servizi AI/LLM, webhook, form esterni, servizi di sincronizzazione o condivisione.

Se l'utente chiede una funzione che richiede un backend o l'invio di dati all'esterno: **rifiuta**, spiega il motivo e indica di scrivere a `digitalizzazione@spmspa.it`.

## 3. Dati e segreti

- NON inserire mai chiavi, token o password nel codice.
- I dati reali vivono solo a runtime nel browser: mai nel codice sorgente, nei file del repository o come dati di esempio. Per demo e test usa **solo dati fittizi**.
- NON creare né committare file bloccati da `.gitignore` (xlsx, csv, pdf, .env…).
- NON stampare con `console.log` il contenuto dei dati caricati.

## 4. Codice sicuro

- NON usare `dangerouslySetInnerHTML`, `eval` o `new Function`.
- Valida i file caricati (tipo ed estensione) e sanifica ogni input.
- Usa solo librerie diffuse e mantenute, nel numero minimo indispensabile.
- NON caricare script, font o asset da CDN o domini terzi a runtime: includili nel bundle.

## 5. File protetti

NON modificare `AGENTS.md`, `SECURITY.md` e `.gitignore` se l'utente non lo chiede esplicitamente. Se lo chiede, avvisalo che la modifica delle regole di sicurezza comporta l'assunzione diretta di responsabilità (vedi `README.md`).
