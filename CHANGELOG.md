# Changelog

Tutte le novità di Energy Grid Tycoon, una versione per volta, dalla più recente.
Formato ispirato a [Keep a Changelog](https://keepachangelog.com/it-IT/1.1.0/); numeri di versione secondo il
[versionamento semantico](https://semver.org/lang/it/) (vedi la sezione «Versioni» del [README](README.md)).

Ogni versione ha queste sezioni, quando servono:
- **Novità**: cose nuove da provare;
- **Modifiche**: cose che funzionano diversamente da prima;
- **Correzioni**: errori sistemati;
- **Da sapere**: salvataggi non compatibili, problemi noti, avvertenze.

## [Non ancora pubblicata]

## [0.8.0-alpha.1] - 2026-11-18

Strade, merci, traffico, perdite di linea, miniere che si esauriscono e nomi. *Roads, freight, traffic, line
losses, mines that run out and names.*

### Novità
- **Strade**: ogni costruzione deve toccare con un lato una **strada collegata al municipio**; senza strada è ferma
  e mostra il segnale «senza strada». All'inizio ci sono già quattro sterrate attorno al municipio.
  - Strumento **Strada** (tasto **R**): clic o trascina per posare le sterrate. Una strada può passare sotto una
    linea elettrica.
  - Strumento **Migliora strada** (tasto **M**): sterrata → strada asfaltata → viale. Ogni livello porta più
    traffico ed è più veloce, ma costa cemento; dopo il miglioramento la casella resta in **cantiere** per qualche
    ora, con meno spazio per il traffico.
  - Demolire una strada rimborsa metà della spesa.
- **Merci sui camion**: carbone, legname, pietra, cemento e cibo non arrivano più da soli in città.
  - Chi produce mette la merce nel suo **piazzale**; i camion la portano al municipio o al **deposito** più vicino,
    e da lì ai **silo** di chi la consuma (le centrali a carbone, il cementificio). Il magazzino frigorifero fa da
    deposito per il cibo.
  - Il municipio ha due camion; ogni **autoparco** ne aggiunge tre. Se i camion non bastano arriva l'avviso
    «Camion insufficienti», i piazzali si riempiono e le costruzioni si fermano («fermo: piazzale pieno»).
  - Il **cibo si rovina** un po' a ogni viaggio: più è lontano, più se ne perde.
- **Traffico**: la mattina i lavoratori vanno al lavoro e il pomeriggio tornano a casa, insieme ai camion.
  - Le strade piene rallentano tutti. I lavoratori in ritardo rendono meno, e il ritardo del giorno prima toglie
    **felicità** (fattore «Traffico dei pendolari»).
  - I **viali** portano molto traffico ma sono rumorosi: tolgono un po' di felicità ai quartieri accanto.
  - **Mappa del traffico** (tasto **G**): colora le strade secondo il carico.
  - Pannello **Trasporti** (tasto **J** o il pulsante in alto): persone e merci in viaggio, tempo medio, camion
    usati, le strade più cariche (un clic le mostra nella Casella) e l'andamento delle ultime 24 ore.
  - La Casella di una strada dice livello, traffico e persone e merci per senso di marcia.
- **Perdite di linea**: l'energia delle centrali si perde lungo le linee fino al **nodo** più vicino, che è il
  municipio o un **trasformatore** (costruzione nuova). Più la centrale è lontana, più perde.
  - Strumento **Migliora linea** (tasto **L**): le linee passano dal livello I al II e al III e perdono meno, ma
    costano **rame**, un materiale nuovo che si compra da fuori.
  - La Casella mostra la perdita di ogni centrale, e il grafico in basso ha una riga per le perdite.
- **Miniere che si esauriscono**: ogni giacimento ha la sua riserva di carbone. Quando sta per finire la miniera
  rende meno, e arrivano gli avvisi «miniera quasi esaurita» e «miniera esaurita». La Casella mostra la riserva e i
  giorni che restano.
- **Laghi**: tre giorni dopo l'esaurimento la miniera sparisce e al suo posto nasce un **lago**. Il lago rinfresca le
  centrali a carbone vicine, che producono un po' di più; fa piacere ai quartieri accanto, come un parco; e ci si
  può pescare.
- **Pompaggio**: una batteria grande, da costruire accanto a un lago.
- **Nomi**: vie, quartieri, ospedali e parchi hanno un nome, e la Casella lo mostra in cima. Col pulsante
  **Rinomina** si cambia; lasciandolo vuoto torna quello automatico. Le strade più cariche nel pannello Trasporti
  hanno il loro nome.
- **Aspetto nuovo**: cornice a cruscotto, pulsanti in rilievo, barra in alto divisa in gruppi, schede della lista
  con il costo in evidenza e il carattere **Barlow Semi Condensed** per titoli e numeri.
- **Trailer nuovo**, con strade e traffico.

### Modifiche
- Si parte con **16 000** di denaro, per pagare le prime strade.
- L'equilibrio del gioco è stato rivisto per le strade, i camion e le perdite di linea: si vince ancora in poco più
  di un anno di gioco, giocando bene.

### Da sapere
- I salvataggi della 0.8.0 hanno un formato nuovo e **non si aprono nelle versioni precedenti**.
- I salvataggi delle versioni precedenti si caricano: il gioco traccia da solo le sterrate attorno al municipio e
  una sterrata verso ogni costruzione; le centrali a carbone ripartono col silo pieno, le miniere con la riserva
  piena, e strade, quartieri, ospedali e parchi ricevono un nome.

## [0.7.0-alpha.1] - 2026-11-16

Salvataggi multipli. *Multiple saves.*

### Novità
- **Salva come…** nel menu di pausa: scegli il nome del salvataggio, oppure sovrascrivi uno di quelli che hai già
  fatto (con una conferma). Fino a 50 salvataggi con nome per partita.
- **Salvataggio rapido**: **F5** salva, **F9** riprende da lì; sul tablet è nel menu di pausa.
- **Salvataggi automatici a rotazione**: uno all'inizio di ogni giorno di gioco, restano gli ultimi tre.
- **Carica partita**, nel menu iniziale e in quello di pausa: i salvataggi raggruppati per partita, con giorno,
  denaro, abitanti e data; si possono caricare, rinominare ed eliminare.
- Nei README: le sezioni **«Prossimamente»** e **«Problemi noti»**.

### Modifiche
- Il pulsante **Salva** in alto crea ogni volta un salvataggio nuovo, col nome «Giorno N»; **Carica** e
  **Continua** riprendono il salvataggio più recente, di qualunque tipo.

### Da sapere
- I salvataggi ora stanno in una cartella per partita. Al primo avvio il gioco trasforma i salvataggi della versione
  precedente in una partita; i file originali restano nella sottocartella `vecchi`. Le versioni precedenti non
  vedono i salvataggi della 0.7.0.

## [0.6.0-alpha.1] - 2026-11-16

Materiali, versione per Android e trailer. *Materials, an Android version and a trailer.*

### Novità
- **Materiali da costruzione**: legname e cemento. Quasi tutte le costruzioni costano, oltre ai soldi, un po' di
  materiali; il costo è scritto sotto il prezzo nella lista e per esteso nel suggerimento.
- **Tre industrie nuove**:
  - **segheria**, solo nel **bosco**: 2 legname all'ora;
  - **cava**, sulle colline: 2 pietra all'ora;
  - **cementificio**, in pianura: trasforma 2 pietra in 2 cemento all'ora.
  Hanno bisogno di personale e di corrente; il cementificio senza pietra si ferma e non consuma energia.
- **Bosco**: un terreno nuovo sulla mappa. Ci si possono posare solo segherie e linee elettriche.
- **Se i materiali mancano** si comprano da fuori al momento della posa (legname 10, cemento 20 l'unità): si può
  giocare anche senza industrie, ma costa di più.
- **Pannello «Scorte»**: il pulsante accanto al carbone, in alto, mostra carbone, legname, pietra, cemento e cibo,
  con quanto entra ed esce all'ora. Si chiude con un clic fuori o con Esc.
- Nel pannello **Casella**: quanto produce e consuma un'industria, e «fermo: manca pietra» quando serve.
- **Versione per Android** (tablet e telefoni con schermo grande, Android 8 o più recente): un file `.apk` da
  installare a mano, fuori dal Play Store. Tocco = clic, tocco lungo = clic destro, due dita per spostare e
  ingrandire la mappa.
- **Trailer** di un minuto, in italiano e in inglese.

### Modifiche
- Si parte con **15 000** crediti invece di 10 000, più 200 di legname e 200 di cemento.

### Da sapere
- **Salvataggi in formato nuovo.** Quelli delle versioni precedenti si caricano con le scorte iniziali di
  materiali; la mappa si ridisegna con i boschi, e le costruzioni finite su un bosco restano al loro posto. I
  salvataggi della 0.6.0 non si aprono con le versioni precedenti.

### In English
- **Building materials**: timber and cement. Most buildings now cost some materials as well as money; the list
  shows them under the price, the tooltip spells them out.
- **Three new industries**: **sawmill** (woods only, 2 timber/h), **quarry** (hills, 2 stone/h) and **cement
  works** (plains, turns 2 stone into 2 cement per hour). They need staff and power; the cement works stops and
  uses no power when it runs out of stone.
- **Woods**: a new terrain; only sawmills and power lines can go there.
- **Missing materials** are bought from outside when you build (timber 10, cement 20 each).
- **Stocks panel**: the button next to coal shows coal, timber, stone, cement and food, with hourly in and out.
- The **Tile** panel shows what an industry produces and uses, and «stopped: no stone».
- **Android version** (tablets and large phones, Android 8 or later): an `.apk` to install by hand, outside the
  Play Store. Tap = click, long press = right-click, two fingers to pan and zoom.
- A one-minute **trailer**, in Italian and English.
- You start with **15,000** credits instead of 10,000, plus 200 timber and 200 cement.
- **New save format**: older saves load with the starting materials and the map gains its woods; buildings that
  end up in the woods stay where they are. 0.6.0 saves don't open in older versions.

## [0.5.0-alpha.1] - 2026-11-15

Felicità, salute e tasse. *Happiness, health and taxes.*

### Novità
- **Felicità leggibile**: va piano verso la somma di alcuni fattori, cioè blackout delle ultime 24 ore, cibo,
  fame, disoccupazione, inquinamento, salute, parchi e tasse. Passando il mouse sul numero si vede quanto pesa
  ognuno. Sotto 35 la gente comincia ad andarsene.
- **Salute**: cala con l'inquinamento e la fame. I malati restano a casa e mancano al lavoro.
- **Ospedale**: cura fino a 250 abitanti; ha bisogno di personale e di corrente.
- **Parco**: alza la felicità, soprattutto in una città piccola.
- **Tasse a tre livelli** (basse, normali, alte): pulsante con la moneta nella barra in alto o tasto **T**.
- Nel pannello **Casella**: la copertura dell'ospedale e la felicità di un parco.
- Luci di notte anche sull'ospedale.

### Modifiche
- I lavoratori vanno all'energia, al cibo, **agli ospedali**, alle miniere e infine ai servizi.
- La città cresce un po' più in fretta, per compensare una felicità che ora sta di solito fra 70 e 85.
- **Barre di scorrimento** della lista delle costruzioni e delle informazioni della Casella: scure e sottili, nello
  stile del gioco.
- Barra in alto più compatta: la data non viene più tagliata nelle lingue con parole lunghe.

### Correzioni
- Il riquadro «Apri il sito dell'autore» non resta più sulla mappa dopo aver lasciato il menu.

### Da sapere
- **Salvataggi in formato nuovo.** Quelli delle versioni precedenti si caricano con tasse normali e salute
  iniziale. I salvataggi della 0.5.0 non si aprono con le versioni precedenti.

### In English
- **Readable happiness**: it moves slowly towards the sum of a few factors (blackouts in the last 24 hours, food,
  hunger, unemployment, pollution, health, parks, taxes); hover over it to see each one. Below 35 people leave.
- **Health**: drops with pollution and hunger; sick people stay home from work.
- **Hospital** (treats up to 250 residents, needs staff and power) and **park** (more happiness, especially in a
  small town).
- **Three tax levels** with the coin button or the **T** key.
- Jobs go to energy, food, **hospitals**, mines, then services. The town grows a little faster.
- Dark, slim **scroll bars**; a more compact top bar, so the date is no longer cut off.
- Fixed: the «Open the author's website» tooltip no longer stays on the map.
- **New save format**: older saves load with normal taxes and starting health; 0.5.0 saves don't open in older
  versions.

## [0.4.0-alpha.2] - 2026-11-15

Correzioni alla 0.4.0-alpha.1. *Fixes for 0.4.0-alpha.1.*

### Correzioni
- Fattoria, peschereccio, serra e magazzino frigorifero **si vedono di nuovo**, sulla mappa e nella lista: nella
  0.4.0-alpha.1 mancava il loro disegno.
- Nella lista delle costruzioni i nomi **non si spezzano più a metà parola**: nome e costo stanno uno sotto
  l'altro, e la barra di scorrimento è più sottile.

### Da sapere
- I salvataggi della 0.4.0-alpha.1 funzionano senza cambiamenti.

### In English
- Farm, fishing boat, greenhouse and cold store **are visible again**, on the map and in the list: their artwork
  was missing in 0.4.0-alpha.1.
- Building names in the list **no longer break mid-word**: name and cost are now stacked, with a thinner scroll bar.
- Saves from 0.4.0-alpha.1 work as they are.

## [0.4.0-alpha.1] - 2026-11-15

La città ha fame: arriva il cibo. *The town gets hungry: food arrives.*

### Novità
- **Il cibo**: gli abitanti mangiano ogni ora. La scorta è nella barra in alto e diventa rossa quando sta per finire.
- **Quattro costruzioni nuove**:
  - **fattoria** (pianura): produce secondo la stagione, niente d'inverno;
  - **peschereccio** (costa): pesca tutto l'anno, ma si ferma col vento troppo forte;
  - **serra** (pianura o collina): produce tutto l'anno, ma consuma molta energia;
  - **magazzino frigorifero** (pianura): la città può tenere più cibo.
- **Il cibo passa dalla rete**: le costruzioni del cibo consumano energia. In un blackout non producono e i
  frigoriferi perdono una parte del cibo in più.
- **Importazione automatica**: se la scorta finisce il cibo arriva da fuori, a caro prezzo. Evita la fame ma non fa
  crescere la città, che per crescere ha bisogno di almeno un giorno di scorta propria. Senza soldi arriva la fame e
  gli abitanti se ne vanno.
- Nel pannello **Casella**: quanto cibo produce una costruzione, quanto spazio aggiunge un frigorifero e quanta
  energia consuma.
- **Luci di notte** anche su serre e frigoriferi.

### Modifiche
- I lavoratori vanno prima all'energia, **poi al cibo**, poi alle miniere, poi ai servizi dei quartieri.
- La disoccupazione pesa un po' di più sulla soddisfazione.
- Tasti da **1 a 9 e 0** per scegliere le costruzioni; il magazzino frigorifero si sceglie dalla lista.
- Lo stato del salvataggio è ora sopra il grafico dell'energia.

### Correzioni
- Con molte costruzioni nella lista la barra in alto e il grafico non vengono più schiacciati.

### Da sapere
- **Salvataggi in formato nuovo.** Quelli delle versioni precedenti si caricano: la città riparte con la scorta di
  cibo iniziale. I salvataggi della 0.4.0 non si aprono con le versioni precedenti.

### In English
- **Food**: residents eat every hour; the stock is in the top bar and turns red when it's low.
- **Four new buildings**: farm (nothing in winter), fishing boat (stops in strong wind), greenhouse (all year, uses
  a lot of power) and cold store (more storage).
- **Food runs on the grid**: food buildings use power, stop in a blackout, and cold stores lose some extra food.
- **Automatic imports** when the stock runs out: expensive, they prevent famine but the town only grows with at
  least a day of its own stock. With no money, famine hits and residents leave.
- Jobs now go to energy, then food, then mines, then services. Unemployment weighs a little more on happiness.
- Keys **1–9 and 0** pick buildings; the cold store is in the list.
- **New save format**: older saves still load with the starting food stock; 0.4.0 saves don't open in older
  versions.

## [0.3.0-alpha.1] - 2026-11-14

**Il gioco ha un nome nuovo: «Voltvale: Energy Grid Tycoon».** *The game has a new name: «Voltvale: Energy Grid Tycoon».*

### Novità
- **Nome e logo nuovi**: Voltvale. «Energy Grid Tycoon» resta come sottotitolo.
- **Tre lingue in più**: tedesco, francese e spagnolo, oltre a italiano e inglese. Al primo avvio il gioco usa la
  lingua del sistema, se è una delle cinque.
- **Il lavoro**: circa il 56 % degli abitanti lavora. Centrali, impianti solari ed eolici e miniere hanno bisogno di
  personale: con poco personale producono meno, senza si fermano (segnale del casco barrato). I lavoratori vanno
  prima all'energia, poi alle miniere, poi ai servizi dei quartieri. La disoccupazione abbassa le tasse e un po' la
  soddisfazione. Nella barra in alto: occupati / forza lavoro; nella casella di ogni edificio: «Personale».
- **Luci di notte**: le finestre di quartieri e municipio si accendono al tramonto e si spengono se manca corrente.

### Modifiche
- La scritta «(in pausa)» compare solo quando il gioco è davvero in pausa.
- A partita iniziata l'avviso di pausa dice «per riprendere».
- Nelle lingue con parole lunghe la barra in alto e il pulsante «Demolisci» non escono più dallo spazio.
- File da scaricare e programmi si chiamano ora `Voltvale` (`Voltvale.exe`, `Voltvale.app`).

### Da sapere
- **Salvataggi**: la cartella ora si chiama «Voltvale». Al primo avvio i salvataggi delle versioni precedenti
  vengono **copiati** dalla cartella «Energy Grid Tycoon», che resta com'era.
- **Lingua**: la scelta fatta nel menu non passa alla versione nuova; al primo avvio vale di nuovo la lingua del
  sistema.
- L'indirizzo della versione web non cambia.
- Le traduzioni tedesca, francese e spagnola sono nuove: segnala pure le frasi strane.

### In English
- **New name and logo**: Voltvale, with «Energy Grid Tycoon» as the subtitle.
- **Three more languages**: German, French and Spanish, alongside Italian and English. On first launch the game
  uses your system language if it's one of the five.
- **Work**: about 56% of residents work. Power plants, solar and wind farms and mines need staff: with too few they
  produce less, with none they stop. Jobs go to energy first, then mines, then district services. Unemployment
  lowers taxes and a little happiness.
- **Night lights** on districts and the town hall, off when there's no power.
- Saves are **copied** from the old «Energy Grid Tycoon» folder on first launch; please pick your language again.

## [0.2.0-alpha.1] - 2026-11-14

Il gioco parla anche inglese. *The game now speaks English too.*

### Novità
- **Inglese**, oltre all'italiano. Nel menu iniziale e in quello di pausa la voce **«Lingua»** cambia lingua al
  volo, senza riavviare la partita.
- Al primo avvio il gioco usa la **lingua del sistema** (italiano su un computer in italiano, inglese altrimenti).
  La scelta fatta nel menu resta salvata.
- Nella versione web si può aprire direttamente una lingua aggiungendo `?lingua=en` o `?lingua=it` all'indirizzo.
- **Date e numeri** seguono la lingua: in inglese «18 Oct 2020», «1,500», «8.0 m/s».

### Modifiche
- Il pannello **«Casella»** è più alto: mostra fino a cinque righe di dettagli senza tagliarle.
- Nel menu iniziale la voce «Esci» è sempre l'ultima.
- Il suggerimento del pulsante ▶/❚❚ ora dice solo «tasto Spazio» (F cambia la velocità).

### Da sapere
- I salvataggi delle versioni precedenti si caricano.
- La traduzione inglese è nuova: se trovi una frase strana o sbagliata, segnalala.

### In English
- **English** is now available alongside Italian. Use **«Language»** in the start menu or the pause menu to switch
  at any time, without restarting.
- On first launch the game picks your **system language**; your choice in the menu is remembered.
- In the web version, add `?lingua=en` to the address to open it straight in English.
- Saves from earlier versions still load. The translation is new: please report anything that reads oddly.

## [0.1.0-alpha.2] - 2026-11-14

Menu, calendario e luce del giorno sulla mappa: il gioco ora ha un inizio, una pausa e un tempo che si legge.

### Novità
- **Menu iniziale** con il logo: Nuova partita, Continua (riprende l'ultimo salvataggio), Esci. Tutorial, livelli,
  sfide e mondo aperto sono segnati «in arrivo». In fondo la versione e il credito, con il link al sito
  dell'autore.
- **Menu di pausa** con **Esc**: Riprendi, Salva ed esci al menu, Nuova partita (con conferma). Il tempo si ferma
  finché il menu è aperto.
- **Calendario**: la partita comincia il **18 ottobre 2020**. In alto si leggono il giorno di gioco, la data e
  l'ora. Le stagioni seguono il calendario: si parte in autunno, l'inverno arriva il 21 dicembre.
- **Stagione nel pannello Meteo**, con la sua icona.
- **Giorno e notte sulla mappa**: la luce cambia con l'ora, e le nuvole scuriscono il cielo.
- **Schermo intero**: il gioco parte a schermo intero; **F11** passa alla finestra e viceversa.
- **Tablet e schermi touch** (versione web): un tocco è un clic, un **tocco lungo** è un clic destro.

### Modifiche
- Le linee elettriche fanno parte dei gruppi di costruzioni attaccate: un gruppo che tocca una linea collegata è
  collegato.
- Testi dell'interfaccia tutti in italiano (per esempio «Produzione dell'ultima ora»).
- L'equilibrio del gioco resta lo stesso: con le stagioni nuove una partita ben giocata si vince più o meno nello
  stesso tempo di prima.

### Da sapere
- I salvataggi della `0.1.0-alpha.1` si caricano: la data si ricava dalle ore già giocate.
- **Esc** annulla prima la costruzione scelta; se non c'è niente da annullare, apre il menu di pausa.
- Le versioni per Windows e macOS non sono ancora state provate su quei sistemi: se qualcosa non va, segnalalo.

## [0.1.0-alpha.1] - 2026-11-13

La prima versione da provare. Si gioca dall'inizio alla fine, ma è un'alpha: ogni segnalazione aiuta.

### Novità
- Mappa con colline, giacimenti di carbone e costa. Si costruiscono linee elettriche, miniere, centrali a carbone,
  pannelli solari, pale eoliche, batterie e quartieri.
- Giorno e notte, stagioni (giornate più corte e più nuvole d'inverno), meteo che cambia, con la previsione delle
  3 ore successive.
- Le costruzioni attaccate fra loro si collegano alla rete insieme: basta che una tocchi una linea o il municipio.
- Segnali sulle costruzioni: «non collegata» e «senza corrente».
- Riquadri informativi al passaggio del mouse su pulsanti, icone e costruzioni.
- Conferma prima di demolire, con lo stato della costruzione e il rimborso.
- Pulsanti per pausa e velocità (1×, 2×, 4×) con icone animate. Il grafico in basso mostra produzione, domanda ed
  energia nelle batterie.
- Obiettivi sempre visibili, schermata di vittoria o sconfitta, salvataggio manuale e automatico ogni giorno.
- Versioni per Windows, macOS e Linux, e una da giocare direttamente nel browser.

### Da sapere
- La partita parte in pausa: premi Spazio o ▶ per iniziare.
- Le versioni per Windows e macOS non sono ancora state provate su quei sistemi: se qualcosa non va, segnalalo.
- Il gioco non è firmato: al primo avvio Windows e macOS chiedono una conferma (vedi «Al primo avvio» nel README).
- In arrivo nelle prossime versioni: la luce del giorno e delle nuvole sulla mappa, lo schermo intero, il menu
  iniziale (arrivati nella `0.1.0-alpha.2`).
