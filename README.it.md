<p align="center">
  <img src="immagini/logo.png" alt="Logo di Voltvale: Energy Grid Tycoon" width="700">
</p>

🇮🇹 Italiano · 🇬🇧 [English](README.md)

# ⚡ Voltvale: Energy Grid Tycoon

[![Ultima versione](https://img.shields.io/github/v/release/scrnetto/energy-grid-tycoon-releases?include_prereleases&label=versione&color=f2c230)](https://github.com/scrnetto/energy-grid-tycoon-releases/releases)
[![Stato](https://img.shields.io/badge/stato-alpha-orange)](#versioni)
[![Gioca nel browser](https://img.shields.io/badge/gioca-nel%20browser-3fae5a)](https://scrnetto.github.io/energy-grid-tycoon-releases/)
[![Piattaforme](https://img.shields.io/badge/piattaforme-Windows%20%7C%20macOS%20%7C%20Linux%20%7C%20Android%20%7C%20Web-3f8fc9)](#scaricare-il-gioco)
[![Ultimo aggiornamento](https://img.shields.io/github/release-date-pre/scrnetto/energy-grid-tycoon-releases?label=ultimo%20aggiornamento&color=3f8fc9)](https://github.com/scrnetto/energy-grid-tycoon-releases/releases)
[![Download](https://img.shields.io/github/downloads/scrnetto/energy-grid-tycoon-releases/total?label=download&color=3f8fc9)](https://github.com/scrnetto/energy-grid-tycoon-releases/releases)
[![Licenza](https://img.shields.io/badge/licenza-gratuito%2C%20tutti%20i%20diritti%20riservati-lightgrey)](LICENSE.md)
[![Lingue](https://img.shields.io/badge/lingue-it%20%7C%20en%20%7C%20de%20%7C%20fr%20%7C%20es-009246)](#lingue)
[![Fatto con Unity](https://img.shields.io/badge/fatto%20con-Unity%206-1d2330?logo=unity)](https://unity.com/)

**Sei il gestore elettrico di una cittadina che cresce.** Ogni ora la città chiede energia: poca di notte, tanta
la sera. Costruisci centrali, impianti solari, parchi eolici e batterie, collega tutto con le linee elettriche,
trova chi ci lavori, dai da mangiare a tutti, produci il legname e il cemento per costruire e fai crescere la città fino a **400 abitanti in due anni di gioco**, senza blackout continui,
senza debiti e senza soffocarla di inquinamento.

Un gioco originale di **Marco Scarlino**. Gratuito.

![Una partita al secondo giorno: attorno al municipio quartieri, impianti solari, parchi eolici, una batteria, una fattoria, una serra, un parco e un ospedale](immagini/schermata-partita.png)

## Trailer

[![Trailer di Voltvale: clic per vedere il video intero di un minuto](immagini/trailer-it.webp)](https://scrnetto.github.io/energy-grid-tycoon-releases/trailer/voltvale-trailer-it.mp4)

**[▶ Guarda il trailer (1 minuto)](https://scrnetto.github.io/energy-grid-tycoon-releases/trailer/voltvale-trailer-it.mp4)** ·
[in inglese](https://scrnetto.github.io/energy-grid-tycoon-releases/trailer/voltvale-trailer-en.mp4)

> **Stato: in sviluppo (alpha).** Il gioco si gioca dall'inizio alla fine, ma mancano ancora molte cose e qualcosa
> può non funzionare. Ogni segnalazione aiuta: vedi [Segnalare un problema o un'idea](#segnalare-un-problema-o-unidea).

## Gioca subito nel browser

**[▶ Gioca a Voltvale nel browser](https://scrnetto.github.io/energy-grid-tycoon-releases/)**: niente da
installare. Serve un browser recente (Chrome, Firefox, Edge, Safari) su un computer con mouse e tastiera, oppure su
un tablet: **tocco = clic, tocco lungo = clic destro**. Clicca sul gioco prima di usare la tastiera. I salvataggi
restano nel browser che usi.

## Scaricare il gioco

Tutte le versioni sono nella pagina **[Releases](../../releases)**. Scarica il file del tuo sistema dall'ultima
versione:

| Sistema | File | Come avviarlo |
|---|---|---|
| **Windows** 10/11 (64 bit) | `Voltvale-<versione>-windows.zip` | Estrai lo zip e apri `Voltvale.exe` |
| **macOS** 12 o successivo | `Voltvale-<versione>-macos.zip` | Estrai lo zip e apri `Voltvale.app` |
| **Linux** (64 bit) | `Voltvale-<versione>-linux.zip` | Estrai lo zip e avvia `Voltvale` |
| **Android** 8 o successivo (tablet o telefono grande) | `Voltvale-<versione>-android.apk` | Apri il file sul dispositivo e installalo (vedi sotto) |

### Al primo avvio

Il gioco non è firmato con un certificato a pagamento, quindi il sistema può avvisarti che viene da uno
sviluppatore sconosciuto. È normale per i giochi indipendenti.

- **Windows**: se compare «Windows ha protetto il PC», clicca **Ulteriori informazioni**, poi **Esegui comunque**.
- **macOS**: se compare «impossibile aprire perché lo sviluppatore non è verificato», fai **clic destro
  sull'app → Apri**, poi conferma con **Apri**. Basta la prima volta. Se il Mac dice che l'app «è danneggiata»,
  apri il Terminale nella cartella dello zip e scrivi `xattr -cr Voltvale.app`.
- **Linux**: se non parte, rendi il file eseguibile con `chmod +x Voltvale`.
- **Android**: il gioco non è sul Play Store. Scarica l'`.apk` sul dispositivo e aprilo; la prima volta Android
  chiede di permettere le installazioni dal browser o dal gestore dei file («Installa app sconosciute»). Play
  Protect può avvisare che l'app è sconosciuta: scegli di installarla comunque. Per aggiornare, installa il nuovo
  `.apk` sopra il vecchio. Sullo schermo touch: **tocco = clic, tocco lungo = clic destro**, due dita per spostare
  la mappa e per ingrandirla.

**Controllare il download (facoltativo).** Ogni versione ha un file `SHA256SUMS.txt` con l'impronta di ogni zip.
Su Linux si controlla con `sha256sum -c --ignore-missing SHA256SUMS.txt`, su macOS con `shasum -a 256 -c SHA256SUMS.txt`.

### Requisiti

- Uno schermo da almeno 1280×800.
- Mouse e tastiera, oppure un tablet (versione web o Android).
- Circa 200 MB di spazio.
- Una scheda video qualsiasi degli ultimi 10 anni: anche quelle integrate vanno bene.

## Come si gioca

Il gioco si apre con il **menu iniziale**: **Nuova partita**, oppure **Continua** per riprendere l'ultimo
salvataggio. La partita comincia il **18 ottobre 2020** e parte **in pausa**: premi **Spazio** per far scorrere il
tempo. A velocità 1× un'ora di gioco dura un secondo, e puoi accelerare a 2× e 4×. Le stagioni seguono il
calendario: si parte in autunno, e d'inverno le giornate sono più corte e il cielo più coperto.

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
  Fa ammalare gli abitanti, e sopra la soglia non si vince.
- **Crescita**: la città cresce se gli abitanti sono abbastanza **felici**, c'è posto nei **quartieri** e c'è abbastanza
  **cibo** in magazzino.

### Lavoro e personale

Le costruzioni hanno bisogno di qualcuno che le faccia funzionare.

- Lavora circa il **56 %** degli abitanti. La barra in alto mostra i posti occupati sulla forza lavoro disponibile.
- **Centrali a carbone**, **impianti solari**, **parchi eolici**, **miniere di carbone**, le **industrie** e le
  costruzioni del **cibo** hanno bisogno di personale. Il pannello **Casella** mostra quanto ne hanno, per esempio **Personale: 8/10**.
- Con poco personale una costruzione produce meno; **senza nessuno si ferma** e mostra il segnale **«senza
  personale»**.
- I lavoratori vanno **prima all'energia**, poi **al cibo**, poi **agli ospedali**, poi **alle industrie**, poi **alle miniere**, poi **ai servizi**
  (quartieri e parchi). I quartieri funzionano anche quando ai loro servizi manca personale.
- La **disoccupazione** fa entrare meno tasse e, se è alta, rende gli abitanti meno felici.

### Cibo

Gli abitanti mangiano ogni ora. La scorta di cibo è nella barra in alto, accanto alla spiga, e diventa rossa quando
sta per finire.

- **Fattoria** (pianura): produce secondo la stagione, molto d'estate e **niente d'inverno**.
- **Peschereccio** (costa): pesca tutto l'anno, ma si ferma quando il vento è troppo forte.
- **Serra** (pianura o collina): produce tutto l'anno, però **consuma molta energia**.
- **Magazzino frigorifero** (pianura): fa crescere la scorta che la città può tenere.
- **Il cibo passa dalla rete**: le costruzioni del cibo consumano energia. Durante un **blackout** non producono e
  i frigoriferi perdono una parte del cibo in più.
- **Se la scorta finisce**, il cibo arriva da fuori in automatico, ma costa caro. Con il cibo importato la città
  non muore di fame, però **non cresce**: per crescere serve almeno un giorno di scorta propria.
- **Se finiscono anche i soldi** arriva la fame, e gli abitanti se ne vanno.
- Il pannello **Casella** mostra quanto produce ogni costruzione (per esempio **Cibo: 2,0/h**), quanto spazio
  aggiunge un frigorifero e quanta energia consuma.

### Felicità, salute e tasse

- **Felicità** (lo smile nella barra in alto): si muove piano verso un valore che è la somma di alcuni fattori, cioè
  blackout delle ultime 24 ore, cibo, fame, disoccupazione, inquinamento, salute, parchi e tasse. Passando il
  mouse sul numero vedi verso quale valore sta andando e quanto pesa ogni fattore, per esempio «Blackout −5,0» o
  «Parchi +3,0». Sotto 60 la città non cresce, e sotto 35 la gente comincia ad andarsene.
- **Salute** (il cuore): cala con l'inquinamento e con la fame. I **malati restano a casa**, quindi ci sono meno
  lavoratori, e una città poco sana è anche meno felice.
- **Ospedale** (pianura): cura fino a 250 abitanti, ha bisogno di personale e consuma energia. Durante un
  blackout non cura. Indispensabile se punti sul carbone.
- **Parco** (pianura o collina): rende la gente più felice. Conta di più in una città piccola: ogni parco vale +3
  ogni 100 abitanti, fino a +10.
- **Tasse**: tre livelli, basse, normali e alte, con il pulsante con la moneta nella barra in alto o il tasto
  **T**. Tasse alte portano più soldi ma meno felicità; tasse basse fanno il contrario.

### Materiali e industrie

Quasi tutte le costruzioni costano, oltre ai soldi, dei **materiali**: **legname** e **cemento**. La lista a
sinistra li mostra sotto il prezzo, con piccole icone; passando il mouse sul pulsante si leggono per esteso.

- **Segheria** (solo nel **bosco**, le caselle verde scuro): 2 legname all'ora.
- **Cava** (colline): 2 pietra all'ora.
- **Cementificio** (pianura): trasforma 2 pietra in 2 cemento all'ora e consuma molta corrente. Senza pietra si
  ferma, e smette anche di consumare corrente.
- Le industrie hanno bisogno di **personale** e di **corrente**. I lavoratori ci vanno dopo energia, cibo e
  ospedali, e prima delle miniere di carbone.
- **Se i materiali non bastano** quando costruisci, la parte che manca si compra subito da fuori (legname 10,
  cemento 20 l'unità). Si può giocare anche senza industrie, ma costa di più.
- Si parte con 200 di legname e 200 di cemento.
- Il pulsante **Scorte**, accanto al carbone nella barra in alto, apre un piccolo pannello con carbone, legname,
  pietra, cemento e cibo, e quanto entra ed esce ogni ora. Si chiude con un clic fuori o con **Esc**.
- Il pannello **Casella** mostra quanto produce e consuma un'industria, e «fermo: manca pietra» quando è finita.

### Comandi

Passa il mouse su qualsiasi icona o pulsante: un riquadro spiega che cos'è. Fermandolo su una costruzione della
mappa vedi il suo stato e quanta energia produce o consuma.

| Comando | Cosa fa |
|---|---|
| Tasti **1–9** e **0** | Scegli cosa costruire: linea elettrica, miniera di carbone, centrale a carbone, impianto solare, parco eolico, batteria, quartiere, fattoria, peschereccio, serra. Magazzino frigorifero, parco e ospedale si scelgono dalla lista a sinistra |
| **Clic sinistro** | Posa la costruzione scelta. Senza nessuna scelta seleziona una casella e ne mostra i dettagli |
| **Clic destro** (sul tablet: tocco lungo) | Con una costruzione scelta, annulla la scelta. Senza scelta, chiede conferma per demolire (rimborso di metà del costo) |
| **Esc** | Annulla la scelta; se non c'è niente da annullare apre il **menu di pausa** (Riprendi, Salva ed esci al menu, Nuova partita, Lingua) |
| **F11** | Schermo intero / finestra |
| **Spazio** o pulsante ▶/❚❚ | Pausa / riprendi |
| **F** o pulsanti delle frecce | Velocità 1×, 2×, 4× |
| **V** | Avanza di un'ora sola |
| **T** o pulsante con la moneta | Tasse basse, normali, alte |
| **WASD** o **frecce**, tasto centrale del mouse | Sposta la vista |
| **Rotella** | Zoom |
| Pulsante **Scorte** (in alto) | Mostra le scorte di carbone, legname, pietra, cemento e cibo |
| **Salva** / **Carica** (in alto) | Salva o riprende la partita. Il gioco salva anche da solo ogni giorno |

### Lingue

Il gioco è in **italiano, inglese, tedesco, francese e spagnolo**. Dal menu iniziale o da quello di pausa la voce
**Lingua** la cambia al volo, senza riavviare la partita, e la scelta resta salvata. Al primo avvio il gioco usa la
lingua del sistema se è una di queste cinque, altrimenti l'inglese. Nella versione web si può aprire direttamente
una lingua aggiungendo `?lingua=it` (oppure `en`, `de`, `fr`, `es`) all'indirizzo.

### Segnali sulle costruzioni

- **Spina staccata** (cerchio bianco e rosso): la costruzione non è collegata alla rete.
- **Fulmine barrato** (cerchio giallo): è collegata ma non riceve corrente (blackout), oppure una centrale a carbone
  è ferma perché il carbone è finito. Una serra o un frigorifero senza corrente non funzionano.
- **Casco barrato** (cerchio azzurro): **senza personale**, la costruzione è ferma. Costruisci altri quartieri o
  libera lavoratori.
- **Luci di notte**: col buio quartieri e municipio accendono le luci. Una costruzione senza corrente resta al
  buio: un quartiere spento di notte è un campanello d'allarme.

### Consigli per la prima partita

1. Metti in pausa e guarda la mappa: le **colline** sono buone per l'eolico, i **giacimenti** scuri servono alle
   miniere.
2. Fai partire una **linea** dal municipio verso dove vuoi costruire.
3. Comincia con un po' di **solare e di eolico** e una **batteria** per la sera.
4. Non costruire troppe centrali tutte insieme: ognuna ha bisogno di **personale**, e la città è ancora piccola.
5. Costruisci **quartieri** man mano che la produzione regge la domanda.
6. Metti presto una **fattoria** e pensa all'inverno: d'inverno le fattorie si fermano, e servono una scorta,
   un peschereccio o una serra.
7. Nel primo mese metti una **segheria** nel bosco e una **cava** su una collina; aggiungi un **cementificio**
   quando hai un po' di soldi da parte. Comprare i materiali da fuori ogni volta costa.
8. Un **parco** presto alza la felicità quando la città è piccola. Se costruisci centrali a carbone, pensa a un
   **ospedale**.
9. Tieni d'occhio il **grafico in basso**: se la linea rossa (domanda) supera la verde (produzione), sta per
   arrivare un blackout.

## Dove finiscono i salvataggi

I salvataggi restano sul tuo computer, o nel tuo browser per la versione web, e il gioco non manda niente su
internet.

- **Windows**: `%USERPROFILE%\AppData\LocalLow\Marco Scarlino\Voltvale\salvataggi`
- **macOS**: `~/Library/Application Support/Marco Scarlino/Voltvale/salvataggi`
- **Linux**: `~/.config/unity3d/Marco Scarlino/Voltvale/salvataggi`
- **Android**: dentro l'app; si cancellano se la disinstalli.

**Arrivi da una versione precedente?** Al primo avvio della 0.3.0 il gioco **copia** i salvataggi dalla vecchia
cartella «Energy Grid Tycoon» (stesso percorso, con «Energy Grid Tycoon» al posto di «Voltvale»). La cartella
vecchia resta dov'è. La **lingua** va scelta di nuovo, una volta sola.

**Dalla 0.4.0** i salvataggi hanno un formato nuovo. Quelli delle versioni precedenti si caricano lo stesso: la
città riparte con la scorta di cibo iniziale. Un salvataggio della 0.4.0 non si apre con le versioni precedenti.

**Dalla 0.5.0** il formato cambia di nuovo: tasse e salute. I salvataggi delle versioni precedenti si caricano con
tasse normali e salute iniziale. Un salvataggio della 0.5.0 non si apre con le versioni precedenti.

**Dalla 0.6.0** il formato cambia ancora: i materiali. I salvataggi delle versioni precedenti si caricano con il
legname e il cemento iniziali, e sulla mappa compaiono i boschi; le costruzioni finite in un bosco restano al loro
posto. Un salvataggio della 0.6.0 non si apre con le versioni precedenti.

I salvataggi di una versione alpha potrebbero non funzionare con la versione successiva: lo scrive il
[changelog](CHANGELOG.md) quando succede.

## Versioni

Le versioni seguono il [versionamento semantico](https://semver.org/lang/it/) con tre fasi:

| Fase | Esempio | Che cosa significa |
|---|---|---|
| **Alpha** | `0.3.0-alpha.1` | Il gioco cambia molto da una versione all'altra; mancano parti; possono esserci errori e salvataggi non compatibili |
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

Voltvale è **gratuito**: puoi scaricarlo e giocarci quanto vuoi. **Non** puoi ridistribuirlo, venderlo o
modificarlo: per farlo giocare a qualcuno, mandagli il link di questa pagina. I dettagli sono in
[LICENSE.md](LICENSE.md).

## Crediti

Ideazione e realizzazione di **Marco Scarlino**, con Unity e con l'aiuto di strumenti di intelligenza artificiale
per il codice, la grafica e le traduzioni.
