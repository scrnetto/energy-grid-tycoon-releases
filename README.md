# ⚡ Energy Grid Tycoon

[![Ultima versione](https://img.shields.io/github/v/release/scrnetto/energy-grid-tycoon-releases?include_prereleases&label=versione&color=f2c230)](https://github.com/scrnetto/energy-grid-tycoon-releases/releases)
[![Stato](https://img.shields.io/badge/stato-alpha-orange)](#versioni)
[![Gioca nel browser](https://img.shields.io/badge/gioca-nel%20browser-3fae5a)](https://scrnetto.github.io/energy-grid-tycoon-releases/)
[![Piattaforme](https://img.shields.io/badge/piattaforme-Windows%20%7C%20macOS%20%7C%20Linux%20%7C%20Web-3f8fc9)](#scaricare-il-gioco)
[![Download](https://img.shields.io/github/downloads/scrnetto/energy-grid-tycoon-releases/total?label=download&color=3f8fc9)](https://github.com/scrnetto/energy-grid-tycoon-releases/releases)
[![Licenza](https://img.shields.io/badge/licenza-gratuito%2C%20tutti%20i%20diritti%20riservati-lightgrey)](LICENSE.md)
[![Lingua](https://img.shields.io/badge/lingua-italiano-009246)](#)
[![Fatto con Unity](https://img.shields.io/badge/fatto%20con-Unity%206-1d2330?logo=unity)](https://unity.com/)

**Sei il gestore elettrico di una cittadina che cresce.** Ogni ora la città chiede energia: poca di notte, tanta
la sera. Costruisci centrali, pannelli solari, pale eoliche e batterie, collega tutto con le linee elettriche e
fai crescere la città fino a **400 abitanti in due anni di gioco**, senza blackout continui, senza debiti e senza
soffocarla di inquinamento.

Un gioco originale di **Marco Scarlino**. Gratuito.

![Una partita al sesto giorno: pannelli solari, pale eoliche e una batteria attorno al municipio](immagini/schermata-partita.png)

> **Stato: in sviluppo (alpha).** Il gioco si gioca dall'inizio alla fine, ma mancano ancora molte cose e qualcosa
> può non funzionare. Ogni segnalazione aiuta: vedi [Segnalare un problema o un'idea](#segnalare-un-problema-o-unidea).

## Gioca subito nel browser

**[▶ Gioca a Energy Grid Tycoon nel browser](https://scrnetto.github.io/energy-grid-tycoon-releases/)**: niente da
installare. Serve un computer con mouse e tastiera e un browser recente (Chrome, Firefox, Edge, Safari). Clicca sul
gioco prima di usare la tastiera. I salvataggi restano nel browser che usi.

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
  municipio e lo allungano, anche in diagonale. Una costruzione è collegata se tocca il municipio, una linea
  oppure un'altra costruzione già collegata: un gruppo di costruzioni attaccate è collegato se una di loro tocca
  la rete.
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

Passa il mouse su qualsiasi icona o pulsante: un riquadro spiega che cos'è. Fermandolo su una costruzione della
mappa vedi il suo stato e quanta energia produce o consuma.

| Comando | Cosa fa |
|---|---|
| Tasti **1–7** | Scegli cosa costruire: linea, miniera, centrale a carbone, solare, eolico, batteria, quartiere |
| **Clic sinistro** | Posa la costruzione scelta. Senza nessuna scelta seleziona una casella e ne mostra i dettagli |
| **Clic destro** | Con una costruzione scelta, annulla la scelta. Senza scelta, chiede conferma per demolire (rimborso di metà del costo) |
| **Esc** | Annulla la scelta |
| **Spazio** o pulsante ▶/❚❚ | Pausa / riprendi |
| **F** o pulsanti delle frecce | Velocità 1×, 2×, 4× |
| **V** | Avanza di un'ora sola |
| **WASD** o **frecce**, tasto centrale del mouse | Sposta la vista |
| **Rotella** | Zoom |
| **Salva** / **Carica** (in alto) | Salva o riprende la partita. Il gioco salva anche da solo ogni giorno |

### Segnali sulle costruzioni

- **Spina staccata** (cerchio bianco e rosso): la costruzione non è collegata alla rete.
- **Fulmine barrato** (cerchio giallo): è collegata ma non riceve corrente (blackout), oppure una centrale a carbone
  è ferma perché il carbone è finito.

### Consigli per la prima partita

1. Metti in pausa e guarda la mappa: le **colline** sono buone per l'eolico, i **giacimenti** scuri servono alle
   miniere.
2. Fai partire una **linea** dal municipio verso dove vuoi costruire.
3. Comincia con un po' di **solare e di eolico** e una **batteria** per la sera.
4. Costruisci **quartieri** man mano che la produzione regge la domanda.
5. Tieni d'occhio il **grafico in basso**: se la linea rossa (domanda) supera la verde (produzione), sta per
   arrivare un blackout.

## Dove finiscono i salvataggi

I salvataggi restano sul tuo computer, o nel tuo browser per la versione web, e il gioco non manda niente su
internet.

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
