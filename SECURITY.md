# Sicurezza - Policy per le app Vibe-Coded

Questa policy vale per tutti i repository creati da questo template.

## 1. Regole di condotta

- Il repository deve essere sempre **Private**, con l'account `digitalizzazione@spmspa.it` aggiunto come collaboratore.
- Accedi a Lovable solo con l'account aziendale (**Google SSO**).
- **Non incollare mai** nei prompt di Lovable dati reali, credenziali o documenti riservati. Per i test usa dati fittizi.
- Non pubblicare né condividere l'app (link pubblico, remix pubblico) senza approvazione di `digitalizzazione@spmspa.it`.
- Non rimuovere né aggirare le regole di `.gitignore` e `AGENTS.md`.

## 2. Dove possono stare i dati aziendali reali

| Dove | Consentito |
|---|---|
| Caricati nell'app in esecuzione, nel tuo browser | ✅ Sì |
| Incollati nella chat o nei prompt di Lovable (finiscono sui server di Lovable) | ❌ No |
| Salvati nel repository GitHub | ❌ No |
| Inviati a servizi esterni (API, cloud, e-mail, AI di terzi) | ❌ No |

Le app sono progettate per elaborare i dati **solo sul tuo computer**: quando carichi un file, questo non lascia il tuo PC.

## 3. Cosa fare se...

**Hai caricato nel repository un file sensibile, o incollato credenziali o dati reali in Lovable:**
1. Non cercare di cancellare tu la cronologia del repository.
2. Se sono coinvolte credenziali (password, chiavi, token), cambiale subito.
3. Scrivi subito all'**ufficio IT**, mettendo in copia (cc) `digitalizzazione@spmspa.it`, con oggetto `[SECURITY]`, indicando: nome del repository, quale dato è coinvolto, quando è successo.

**Hai notato un comportamento sospetto o una vulnerabilità in un'app:**
- Segnalalo in privato all'ufficio IT, mettendo in copia (cc) `digitalizzazione@spmspa.it`, con oggetto `[SECURITY]`, descrivendo cosa hai visto e come riprodurlo.
- Non aprire issue pubbliche e non parlarne in canali condivisi.

## 4. Responsabilità

La modifica o la rimozione delle regole di sicurezza di questo template comporta l'assunzione diretta di responsabilità da parte dell'utente (vedi `README.md`).

## Contatti

In caso di incidente o sospetta vulnerabilità, scrivi all'**ufficio IT** mettendo in copia (cc):

📧 `digitalizzazione@spmspa.it`
