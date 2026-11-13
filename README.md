# Generatore Orario

Programma per costruire e gestire l'orario settimanale di una scuola secondaria italiana: generazione automatica,
correzione a mano nell'editor, pubblicazione, export verso il registro elettronico e gestione giornaliera delle
supplenze, con monitor nei plessi e app per i docenti.

Questo repository contiene **solo le versioni pubblicate** (pacchetti compilati e manifesto firmato degli
aggiornamenti). I programmi installati si aggiornano da qui da soli. Il codice sorgente non è pubblico.

## Cosa fa

- **Orario automatico** con le regole della scuola italiana: cattedre e monte ore, disponibilità e giorni liberi,
  ore buche, plessi e trasferimenti, palestre e laboratori, scansione delle discipline, compresenze, sostegno,
  desiderata dei docenti con ordine di precedenza. Prima cerca un orario che rispetti tutte le regole, poi
  soddisfa il più possibile i desiderata; un verificatore indipendente ricontrolla ogni orario prodotto.
- **Editor a trascinamento** con conflitti in tempo reale, stampe PDF, griglie Excel, pagina di pubblicazione,
  export per ClasseViva/ZonabitOrario, importazione di orari fatti con aSc Orari e ODIweb.
- **Supplenze del giorno**: proposte ordinate per opportunità ed equità (ore a disposizione, recupero, banca oraria,
  eccedenti), monitor per ogni plesso, archivio, avvisi ai supplenti, calendario d'istituto.
- **App dei docenti** (pagina web installabile su iPhone e Android): orario personale, supplenze con presa visione,
  segnalazione delle assenze, notifiche.
- **Database comune** sul server della scuola: i dati restano nella scuola, con copie giornaliere e, se si vuole,
  copie cifrate su Google Drive.

## Quale pacchetto scaricare

Nella pagina dell'ultima versione (*Releases*, a destra):

| Pacchetto | Per | Sistemi |
| --- | --- | --- |
| `solver` | il PC di chi fa l'orario (generatore, editor, anche supplenze) | Windows, macOS, Linux |
| `vicepresidenza` | i PC delle supplenze e dei monitor | Windows, macOS, Linux |
| `server` | il server della scuola (database comune, app dei docenti) | Windows, macOS, Linux |

Su Windows conviene l'**installatore** (`…-installatore-windows.exe`); su macOS e Linux lo zip del proprio sistema
(`macos-arm64` per i Mac con chip Apple, `macos-x64` per i Mac Intel). Python e le librerie sono già inclusi: non
serve installare nient'altro. In ogni pacchetto il file `LEGGIMI.txt` riassume i primi passi; il manuale completo è
in `documenti/` e si apre anche dal programma (link «Manuale»).

## Prova e licenza

Senza licenza il programma funziona in prova per 20 giorni. Il software è proprietario: l'uso è regolato dalla
licenza contenuta in ogni pacchetto (`documenti/LICENZA.txt`).

Autore: Francesco Rocchi. Informazioni, licenze e assistenza: francesco.rocchi89@gmail.com (risposta entro 72 ore).
