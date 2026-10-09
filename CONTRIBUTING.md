# Come contribuire

Regole comuni a tutti i repository di **DAI_VITE**, un'org **condivisa**: ci lavorano
persone di organizzazioni diverse. Un repository può aggiungere regole proprie nel suo
`CONTRIBUTING.md`, mai toglierne.

## Titolarità e limiti

- La titolarità dei contenuti segue gli accordi fra le parti; i membri trovano titolare e
  accordo nel profilo per i membri (repo `.github-private`). Questo file è pubblico e non li
  nomina. Contribuire non cambia la titolarità.
- **Non si caricano**: credenziali e segreti, dati personali non previsti dagli accordi, dati
  economici, documenti contrattuali, materiale di terzi senza licenza compatibile.
- A fine progetto i repository si consegnano o archiviano secondo gli accordi e gli accessi di
  chi esce si rimuovono.

## Prima di cominciare

- Il README del repository dice a cosa serve, chi ne è responsabile e come si avvia.
- Per un lavoro non banale apri prima una issue (modulo «Bug» o «Richiesta»).

## Lingua

- **Inglese** per commit, nomi dei rami, codice, commenti e nomi delle etichette.
- **Italiano** per i testi rivolti alle persone: issue, descrizioni delle pull request,
  documentazione, note di rilascio.

## Rami

- Nome `tipo/descrizione-breve` (es. `feat/export-csv`) oppure `<attività>/<argomento>` quando
  il ramo segue un'attività del progetto (es. `or1/data-ingestion`).
- Minuscole e trattini; un ramo per argomento; si cancella dopo il merge (automatico).

## Commit

Formato [Conventional Commits 1.0.0](https://www.conventionalcommits.org/en/v1.0.0/):
`<type>(<scope>): <summary>`, sommario **≤72 caratteri** all'imperativo, corpo sul **perché**,
collegamento a issue e PR (`Closes #n`). Firma dei commit raccomandata (sul piano Free dei repo
privati non si può imporre: disciplina e audit).

### Uso di strumenti AI

I messaggi di commit e le descrizioni delle PR **non contengono attribuzioni a strumenti AI**: niente `Co-authored-by:` di assistenti, niente «Generated with …». Chi firma il commit risponde del contenuto, comunque lo abbia prodotto.

## Pull request

- Titolo in formato Conventional Commits (≤72 caratteri, inglese): con lo squash merge diventa
  il commit su `main`.
- Descrizione in italiano: cosa, perché, come si verifica. Almeno un'etichetta `type:`.
- Merge solo **squash**; il ramo si cancella da solo.

## Versioni e rilasci

- **Codice**: [SemVer 2.0.0](https://semver.org/lang/it/), tag `vX.Y.Z`, note di rilascio automatiche
  raggruppate per etichetta (`.github/release.yml`).
- **Documenti da consegnare**: tag `<codice attività>-v<n>` (es. `1.1-v1`), come descritto nel
  `come-contribuire.md` del repository; i tag non si spostano né si cancellano.

## Segreti caricati per errore

Avvisa subito chi è indicato in [SECURITY](SECURITY.md): il segreto va revocato, cancellare il
file non basta.
