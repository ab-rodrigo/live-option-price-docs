# Live Option Price for OpenCart 3.x / 4.x

![Versione OpenCart](https://img.shields.io/badge/OpenCart-4.x-blue?style=for-the-badge&logo=opencart)
![Versione OpenCart](https://img.shields.io/badge/OpenCart-3.x-blue?style=for-the-badge&logo=opencart)
![Licenza](https://img.shields.io/badge/License-GPL--3.0-green?style=for-the-badge)
![Lingue](https://img.shields.io/badge/Languages-5-orange?style=for-the-badge)

[English](README.md) | [Português (BR)](README.pt-br.md) | [Português (PT)](README.pt-pt.md) | [Español](README.es-es.md) | [Français](README.fr-fr.md) | [Italiano](README.it-it.md)

![Live Option Price](./assets/images/social_preview.png)

[![Download](./assets/images/pt-br/download.png)](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)

---

## Informazioni

### Panoramica

<p align="center">
  <img src="./assets/images/demo-price-animation.gif" width="20%" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="./assets/images/demo-fade-effect.gif" width="20%" />
</p>

**Live Option Price** aggiorna il prezzo del prodotto in tempo reale quando il cliente seleziona le proprie opzioni, modifica la quantità o cambia altre informazioni relative al prodotto.

Senza il modulo, il prezzo visualizzato sulla pagina del prodotto potrebbe rimanere invariato finché il cliente non completa un'azione aggiuntiva. Con **Live Option Price**, i valori vengono ricalcolati automaticamente e presentati direttamente sulla pagina del prodotto.

Il modulo utilizza i valori configurati nativamente in OpenCart, tra cui:

- Prezzo del prodotto.
- Prezzo delle opzioni.
- Sconti.
- Prezzo speciale.
- Tasse.
- Punti del prodotto e delle opzioni, se abilitati.
- Quantità selezionata.

Il risultato viene presentato direttamente sulla pagina del prodotto, offrendo al cliente una visualizzazione immediata del valore corrispondente alla configurazione scelta.

### Compatibilità

**Live Option Price** è stato sviluppato per funzionare con le seguenti versioni:

- **OpenCart 3.x**
- **OpenCart 4.x**

L'interfaccia di amministrazione e il funzionamento possono presentare lievi differenze visive tra le versioni di OpenCart, ma le funzionalità e le configurazioni del modulo rimangono le stesse.

---

## Requisiti

Assicurati di disporre delle autorizzazioni amministrative per:

- **Programma di installazione estensioni**
- **Estensioni / Moduli**
- **Modifiche**
- **Configurazione del modulo**

> **Importante:** l'installazione deve essere eseguita utilizzando il file ufficiale del modulo fornito per la tua versione di OpenCart.

---

## Caratteristiche principali

| Caratteristica | Descrizione |
| :--- | :--- |
| **Prezzo in tempo reale** | Aggiorna automaticamente il prezzo quando il cliente modifica le opzioni del prodotto. |
| **Prezzi delle opzioni** | Tiene conto dei rincari e degli sconti definiti nelle opzioni del prodotto. |
| **Sconti per quantità** | Considera automaticamente gli sconti per quantità configurati in OpenCart. |
| **Prezzo speciale** | Mantiene il calcolo compatibile con il prezzo speciale del prodotto. |
| **Moltiplica per la quantità** | Consente di visualizzare il valore totale in base alla quantità selezionata. |
| **Prezzo unitario** | Visualizza il prezzo corrispondente a un'unità quando il cliente seleziona più di un'unità. |
| **Badge di sconto** | Mostra visivamente la percentuale di sconto applicata al prodotto. |
| **Tasse** | Aggiorna le informazioni sui prezzi relative alle tasse in base alle impostazioni fiscali di OpenCart. |
| **Punti** | Aggiorna i punti visualizzati per il prodotto in base alle opzioni selezionate e alla quantità. |
| **Animazione di conteggio** | Anima il cambiamento numerico del prezzo durante gli aggiornamenti. |
| **Effetto opacità (Fade)** | Applica una transizione visiva durante l'aggiornamento del prezzo. |

---

> **Importante:** il modulo non sostituisce le impostazioni dei prezzi di OpenCart. Utilizza i valori esistenti nel prodotto, nelle opzioni, negli sconti e nelle impostazioni fiscali del negozio per eseguire il calcolo.

---

## Installazione

Segui il flusso sottostante per installare il modulo:

1. **Download**: Ottieni il modulo ufficiale direttamente dall'[OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr).
2. **Upload**: Nel pannello di amministrazione del tuo negozio, vai a **Estensioni > Programma di installazione**, clicca su **Upload** e seleziona il file scaricato.
3. **Attivazione**: Individua il modulo nell'elenco delle estensioni e clicca sull'icona **Installa** per attivarlo.

> **Suggerimento tecnico**: Dopo l'attivazione, ricordati di andare su **Estensioni > Modifiche** e cliccare sul pulsante **Aggiorna (Refresh)** (icona blu) per cancellare la cache del sistema.

---

## Accesso alle configurazioni

Dopo aver installato il modulo:

1. Vai a **Estensioni > Estensioni**.
2. Filtra per **Moduli**.
3. Individua **Live Option Price**.
4. Clicca su **Modifica**.

---

# Configurazioni

![Configurazione](./assets/images/pt-br/docs-config-pt-br.png)

| Parametro | Funzione |
|---|---|
| **Moltiplica per la quantità** | Determina se il prezzo visualizzato deve considerare la quantità selezionata dal cliente.<br>**Importante:** questa impostazione controlla in modo specifico il modo in cui viene presentato il prezzo. La quantità continua ad essere considerata da OpenCart nelle altre operazioni applicabili. |
| **Mostra badge di sconto** | Visualizza un badge con la percentuale di sconto quando il prodotto ha un prezzo promozionale o uno sconto per quantità applicabile.<br>**Importante:** la percentuale presentata è calcolata dal modulo in base alla differenza tra il prezzo di riferimento e il prezzo scontato applicato. |
| **Mostra prezzo unitario** | Visualizza il valore corrispondente a un'unità del prodotto quando la quantità selezionata è maggiore di 1. Il prezzo unitario viene visualizzato quando il calcolo è impostato per considerare la quantità e la quantità selezionata è superiore a un'unità.<br>**Nota:** questa funzione aggiorna solo dinamicamente le informazioni presentate nella pagina del prodotto. Le regole dei punti di OpenCart rimangono la fonte dei valori utilizzati dal modulo. |
| **Calcola punti** | Se abilitato, il modulo aggiorna dinamicamente i punti visualizzati sulla pagina del prodotto in base alle opzioni selezionate. I valori delle opzioni possono avere le proprie impostazioni dei punti in OpenCart. |
| **Animazione di conteggio** | Anima il cambiamento numerico del prezzo durante gli aggiornamenti. I numeri vengono animati durante la transizione invece di essere semplicemente sostituiti. Questa opzione è puramente visiva e può essere utilizzata per fornire una transizione più fluida tra i valori. |
| **Effetto opacità (Fade)** | Applica una transizione di opacità visiva durante l'aggiornamento del prezzo. L'effetto aiuta a indicare visivamente che il valore è in fase di aggiornamento dopo una modifica delle opzioni o della quantità.<br>**Importante:** quando l'**Animazione di conteggio** è abilitata, il modulo dà priorità all'animazione numerica del prezzo rispetto all'effetto opacità.|
| **Stato** | Abilita o disabilita il modulo. |

---

# Utilizzo sulla pagina del prodotto

Una volta che il modulo è installato, attivo e configurato, non è richiesta alcuna ulteriore azione.

Accedendo alla pagina di un prodotto, il prezzo viene calcolato automaticamente.

---

# Compatibilità dei temi

Il modulo aggiorna gli elementi di prezzo esistenti sulla pagina del prodotto e funziona con la struttura predefinita del catalogo di OpenCart.

Poiché i temi di terze parti possono modificare la struttura HTML della pagina del prodotto, la presentazione visiva può variare a seconda del tema utilizzato.

> **Importante:** il funzionamento dei calcoli è indipendente dall'aspetto del tema. Se un tema altera significativamente la struttura predefinita della pagina del prodotto, potrebbe essere necessario un adattamento specifico per quel tema. Se necessario, contatta il supporto.

---

# Risoluzione dei problemi

## Il prezzo non si aggiorna

Controlla:

1. Se il modulo è installato.
2. Se il modulo ha lo **Stato = Abilitato**.
3. Se l'estensione è abilitata in OpenCart.
4. Se le modifiche sono state aggiornate dopo l'installazione.
5. Se la cache di OpenCart è stata svuotata.
6. Se la cache del tema è stata svuotata, dove applicabile.
7. Se l'opzione del prodotto ha una variazione di prezzo configurata.

---

## Il prezzo dell'opzione non appare correttamente

Verifica la configurazione dell'opzione direttamente nella registrazione del prodotto.

Conferma:

- Valore dell'opzione.
- Prefisso del prezzo.
- Prodotto associato all'opzione.
- Opzione selezionata sulla pagina del prodotto.

**Live Option Price** utilizza le informazioni registrate in OpenCart per eseguire il calcolo.

---

## Il prezzo non cambia alterando la quantità

Verifica se: **Moltiplica per la quantità** è abilitato nelle impostazioni del modulo. Conferma inoltre se il tema utilizza correttamente il campo quantità predefinito di OpenCart.

---

## Lo sconto per quantità non appare

Conferma se esiste una regola di sconto registrata per:

- il prodotto;
- il gruppo di clienti;
- la quantità selezionata;
- il periodo attuale.

Verifica anche la priorità delle regole di sconto configurate in OpenCart.

---

## Il badge di sconto non appare

Conferma se: **Mostra badge di sconto** è abilitato. Il badge viene visualizzato solo quando è applicabile una percentuale di sconto.

---

## Il prezzo unitario non appare

Conferma se: **Mostra prezzo unitario** è abilitato. È inoltre necessario che il calcolo stia considerando la quantità e che la quantità selezionata sia superiore a un'unità.

---

# Pulizia della cache

Dopo l'installazione o l'aggiornamento del modulo, si consiglia di aggiornare le cache di OpenCart.
Vai a: **Estensioni > Modifiche** e clicca su: **Aggiorna (Refresh)**. Svuota anche la cache del tema, quando questa funzione è disponibile nella tua installazione.

> **Suggerimento:** se una modifica apportata nel modulo non viene visualizzata immediatamente, il primo passo diagnostico dovrebbe essere la pulizia delle cache.

---

## Disinstallazione

Segui i passaggi seguenti per eseguire una disinstallazione pulita e sicura:

1. **Disinstalla**: Vai a **Estensioni > Estensioni**, filtra per **Moduli**, individua il modulo e clicca su **Disinstalla (Uninstall)**.
2. **Elimina**: Individua il modulo nell'elenco delle estensioni installate e clicca sull'icona **Elimina (Delete)**.

> **Cosa succede ai dati?**: La disinstallazione rimuove solo le impostazioni e i file del modulo.

---

# Supporto

In caso di problemi durante l'installazione o l'utilizzo di **Live Option Price**, utilizza la pagina ufficiale dell'estensione su OpenCart Marketplace.

### Prima di richiedere supporto

Per facilitare la diagnosi, fornisci:

- Versione di OpenCart.
- Versione di PHP.
- Tema utilizzato.
- Versione di Live Option Price.
- Descrizione del problema.
- Passaggi per riprodurre il problema.

Ove possibile, includi screenshot delle impostazioni e della pagina del prodotto.

### Ottieni supporto

[Ottieni supporto tramite l'OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)

---

## Ti piace il modulo?

Se **Live Option Price** sta aiutando il tuo negozio e migliorando l'esperienza dei tuoi clienti, prendi in considerazione l'idea di offrire un caffè all'autore.

Questo aiuta a mantenere lo sviluppo, la manutenzione e i futuri aggiornamenti del progetto.

[![Buy me a coffee](./assets/images/pt-br/buy_me_a_coffee.png)](https://www.paypal.com/donate/?hosted_button_id=SPQH2B32XBJUW)

---

## Informazioni sulla licenza

Questa estensione è concessa in licenza ai sensi della **GNU General Public License v3.0 (GPL-3.0)**.

- L'uso e la modifica del software devono essere conformi ai termini stabiliti dalla licenza GPL-3.0.
- Il supporto tecnico e gli aggiornamenti vengono forniti esclusivamente agli acquirenti originali tramite il Marketplace ufficiale di OpenCart.
- Per i dettagli completi della licenza, consulta il file **LICENSE** distribuito con l'estensione o visita la pagina ufficiale della [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).

---

© 2026 **Rodrigoab** · [OpenCart Extensions](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)