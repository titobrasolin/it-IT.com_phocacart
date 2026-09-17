# it-IT.com_phocacart

Traduzione italiana per [PhocaCart](https://www.phoca.cz/phocacart), a partire dal [pacchetto ufficiale generato dall'IA](https://github.com/PhocaCz/PhocaCart/releases/download/languages/it-IT_com_phocacart_ai_lang_2026-02-02.zip) (`it-IT_com_phocacart_ai_lang_2026-02-02.zip`), corretta e mantenuta nel tempo.

Le traduzioni ufficiali di Phoca per questa lingua sono generate automaticamente da un'IA e risultano in alcuni punti imprecise o troppo letterali. Questo repository parte da quel pacchetto e lo affina progressivamente, restando comunque installabile come un normale file di lingua Joomla.

## Installazione manuale

1. Vai alla pagina [Releases](../../releases) e scarica l'ultimo file `it-IT_com_phocacart_lang_*.zip`.
2. In Joomla: **Sistema → Gestisci → Installa** → carica lo zip.

## Aggiornamenti automatici da Joomla (consigliato)

Il pacchetto include nel manifesto il proprio *update site*, rigenerato automaticamente ad ogni release:

```
https://raw.githubusercontent.com/titobrasolin/it-IT.com_phocacart/main/update.xml
```

Dopo aver installato **una prima volta** lo zip da questo repository (vedi sopra), Joomla registra da solo questo sito di aggiornamento: da quel momento in poi le nuove versioni vengono segnalate automaticamente in **Sistema → Gestisci → Aggiornamenti**, senza bisogno di configurare nulla.

Joomla non permette di aggiungere manualmente un nuovo sito di aggiornamento dalla pagina **Sistema → Gestisci → Siti di aggiornamento** (non esiste un pulsante "Nuovo": quell'elenco mostra solo le voci già registrate dalle estensioni installate). Se hai già installato il pacchetto originale di Phoca, per agganciarti agli aggiornamenti di questa traduzione devi installare lo zip di questo repository **in sovrascrittura** sopra quello esistente: l'installazione registrerà automaticamente il sito di aggiornamento, che da quel momento comparirà nell'elenco e potrai eventualmente modificarne l'URL con l'icona a matita.

## Come nascono le release

Ogni modifica ai file di traduzione (`it-IT.com_phocacart.ini`, `.sys.ini`, `.xml`) pushata su `main` fa scattare una GitHub Action che:

1. incrementa la versione nel manifesto XML;
2. impacchetta i file in un nuovo zip installabile;
3. pubblica una nuova [Release](../../releases) con lo zip allegato;
4. rigenera `update.xml` in modo che punti sempre all'ultima release.

Vedi [`.github/workflows/release.yml`](.github/workflows/release.yml).

## Attribuzione

Traduzione originale: Phoca | Jan Pavelka | [phoca.cz](https://www.phoca.cz) — generata con IA e qui rifinita manualmente.
