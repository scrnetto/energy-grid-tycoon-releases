# ⚡ Energy Grid Tycoon

**Sei il gestore elettrico di una cittadina che cresce.** Ogni ora la città chiede energia: poca di notte, tanta
la sera. Costruisci centrali, pannelli solari, pale eoliche e batterie, collega tutto con le linee elettriche e
fai crescere la città fino a **400 abitanti in due anni di gioco**, senza blackout continui, senza debiti e senza
soffocarla di inquinamento.

Un gioco originale di **Marco Scarlino**. Gratuito.

![Una partita appena iniziata](immagini/schermata-partita.png)

> **Stato: in sviluppo (alpha).** Il gioco si gioca dall'inizio alla fine, ma mancano ancora molte cose e qualcosa
> può non funzionare. Ogni segnalazione aiuta: vedi [Segnalare un problema o un'idea](#segnalare-un-problema-o-unidea).

## Scaricare il gioco

Tutte le versioni sono nella pagina **[Releases](../../releases)**. Scarica il file del tuo sistema dall'ultima
versione:

| Sistema | File | Come avviarlo |
|---|---|---|
| **Windows** 10/11 (64 bit) | `EnergyGridTycoon-<versione>-windows.zip` | Estrai lo zip e apri `EnergyGridTycoon.exe` |
| **macOS** 12 o successivo | `EnergyGridTycoon-<versione>-macos.zip` | Estrai lo zip e apri `EnergyGridTycoon.app` |
| **Linux** (64 bit) | `EnergyGridTycoon-<versione>-linux.zip` | Estrai lo zip e avvia `EnergyGridTycoon` |

### Al primo avvio

Il gioco non è firmato con un certificato a pagamento, quindi il sistema può avvisarti che viene da uno
sviluppatore sconosciuto. È normale per i giochi indipendenti.

- **Windows**: se compare «Windows ha protetto il PC», clicca **Ulteriori informazioni**, poi **Esegui comunque**.
- **macOS**: se compare «impossibile aprire perché lo sviluppatore non è verificato», fai **clic destro
  sull'app → Apri**, poi conferma con **Apri**. Basta la prima volta. Se il Mac dice che l'app «è danneggiata»,
  apri il Terminale nella cartella dello zip e scrivi `xattr -cr EnergyGridTycoon.app`.
- **Linux**: se non parte, rendi il file eseguibile con `chmod +x EnergyGridTycoon`.

**Controllare il download (facoltativo).** Ogni versione ha un file `SHA256SUMS.txt` con l'impronta di ogni zip.
Su Linux e macOS si controlla con `sha256sum -c SHA256SUMS.txt` (su macOS `shasum -a 256 -c SHA256SUMS.txt`).

### Requisiti

- Uno schermo da almeno 1280×800.
- Mouse e tastiera.
- Circa 200 MB di spazio.
- Una scheda video qualsiasi degli ultimi 10 anni: anche quelle integrate vanno bene.

## Come si gioca

La partita parte **in pausa**: premi **Spazio** per far scorrere il tempo. A velocità 1× un'ora di gioco dura un
secondo, e puoi accelerare a 2× e 4×.

- **Obiettivo**: arrivare a **400 abitanti** con l'inquinamento **sotto la soglia** entro **2 anni**.
- **Sconfitta**: se resti in rosso con i soldi per **30 giorni di fila**, oppure se finiscono i 2 anni.
- **La rete**: ogni costruzione deve essere collegata al **municipio**. Le **linee elettriche** partono dal
  municipio e lo allungano, anche in diagonale. Una costruzione è collegata se tocca il municipio o una linea.
  I **quartieri** si collegano anche toccando altri quartieri già collegati.
- **Domanda ed energia**: la città consuma poco di notte e molto la sera, verso le 19. Se l'energia non basta
  c'è il **blackout**: gli abitanti si arrabbiano e qualcuno se ne va.
- **Le fonti**:
  - il **sole** produce solo di giorno, poco d'inverno e col cielo coperto;
  - il **vento** cambia di ora in ora;
  - il **carbone** produce sempre, ma inquina e consuma il carbone estratto dalle **miniere**.
- **Batterie**: accumulano l'energia in più e la restituiscono quando serve, per esempio la sera.
- **Il surplus** si vende alla rete esterna, ma più ne offri e meno vale.
- **Inquinamento**: le centrali a carbone inquinano e l'aria si pulisce piano. Una centrale si regge, troppe no.
  Sopra la soglia la gente è scontenta e la città smette di crescere.
- **Crescita**: la città cresce se gli abitanti sono contenti e c'è posto nei **quartieri**.

### Comandi

| Comando | Cosa fa |
|---|---|
| Tasti **1–7** | Scegli cosa costruire: linea, miniera, centrale a carbone, solare, eolico, batteria, quartiere |
| **Clic sinistro** | Posa la costruzione scelta. Senza nessuna scelta mostra i dettagli della casella |
| **Clic destro** | Demolisce la costruzione sotto il mouse (ti rimborsa metà del costo) |
| **Esc** | Annulla la scelta |
| **Spazio** | Pausa / riprendi |
| **F** | Velocità 1× → 2× → 4× |
| **V** | Avanza di un'ora sola |
| **WASD** o **frecce**, tasto centrale del mouse | Sposta la vista |
| **Rotella** | Zoom |
| **Salva** / **Carica** (in alto) | Salva o riprende la partita. Il gioco salva anche da solo ogni giorno |

### Consigli per la prima partita

1. Metti in pausa e guarda la mappa: le **colline** sono buone per l'eolico, i **giacimenti** scuri servono alle
   miniere.
2. Fai partire una **linea** dal municipio verso dove vuoi costruire.
3. Comincia con un po' di **solare e di eolico** e una **batteria** per la sera.
4. Costruisci **quartieri** man mano che la produzione regge la domanda.
5. Tieni d'occhio il **grafico in basso**: se la linea rossa (domanda) supera la verde (produzione), sta per
   arrivare un blackout.

## Dove finiscono i salvataggi

I salvataggi restano sul tuo computer e il gioco non manda niente su internet.

- **Windows**: `%USERPROFILE%\AppData\LocalLow\Marco Scarlino\Energy Grid Tycoon\salvataggi`
- **macOS**: `~/Library/Application Support/Marco Scarlino/Energy Grid Tycoon/salvataggi`
- **Linux**: `~/.config/unity3d/Marco Scarlino/Energy Grid Tycoon/salvataggi`

I salvataggi di una versione alpha potrebbero non funzionare con la versione successiva: lo scrive il
[changelog](CHANGELOG.md) quando succede.

## Versioni

Le versioni seguono il [versionamento semantico](https://semver.org/lang/it/) con tre fasi:

| Fase | Esempio | Che cosa significa |
|---|---|---|
| **Alpha** | `0.1.0-alpha.1` | Il gioco cambia molto da una versione all'altra; mancano parti; possono esserci errori e salvataggi non compatibili |
| **Beta** | `0.9.0-beta.1` | Tutte le parti principali ci sono; si sistemano errori ed equilibrio del gioco |
| **Stabile** | `1.0.0` | La prima versione completa. Poi `1.0.1` per le correzioni e `1.1.0` per le novità |

Le versioni alpha e beta sono segnate su GitHub come **pre-release**. Cosa cambia in ogni versione è nel
**[CHANGELOG](CHANGELOG.md)** e nella pagina di ogni release.

## Segnalare un problema o un'idea

Apri una segnalazione nella pagina **[Issues](../../issues/new/choose)** e scegli:
- **Problema**: qualcosa non funziona. Scrivi cosa stavi facendo, cosa ti aspettavi e la versione del gioco.
- **Idea**: una proposta per migliorare il gioco.

Serve un account GitHub, che è gratuito. Se non ce l'hai, scrivi pure a Marco direttamente.

## Licenza

Energy Grid Tycoon è **gratuito**: puoi scaricarlo e giocarci quanto vuoi. **Non** puoi ridistribuirlo, venderlo
o modificarlo: per farlo giocare a qualcuno, mandagli il link di questa pagina. I dettagli sono in
[LICENSE.md](LICENSE.md).

## Crediti

Ideazione e design di **Marco Scarlino**. Realizzato con Unity, con l'aiuto di strumenti di intelligenza
artificiale per il codice e la grafica.
