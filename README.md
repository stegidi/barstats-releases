# Ciao! Benvenuto su BarStats 📊

Ho creato **BarStats** (prima si chiamava *TempBar*) per tenere d'occhio il mio Mac senza dover aprire Monitoraggio Attività ogni volta.

Con BarStats hai tutto a colpo d'occhio, direttamente nella barra dei menu:
* Scegli fino a **3 valori live** da mostrare in alto: **temperatura, CPU, RAM, GPU, disco, rete e ventole**.
* Clicca sull'icona per aprire il menu: vedi **tutte le metriche insieme** e, toccando le tessere della griglia, decidi quali tenere in barra. Nella riga **«In barra»** trascini gli elementi per sceglierne l'ordine.
* Non serve nessuna password né `sudo`, e quando lo schermo è spento l'app si mette in pausa per non consumare nulla.

**Bonus per chi usa Claude Code:** puoi attivare un **granchietto** 🦀 in pixel art che ti mostra lo stato delle tue sessioni (sta lavorando, aspetta un tuo permesso, ha finito). Se Claude avvia dei subagenti, dei granchietti viola gli girano intorno, uno per agente, e nel menu vedi cosa sta facendo ciascuno.

---

### 🚀 Download e Primo Avvio (Cosa fare)

👉 **[Scarica l'ultima versione di BarStats (.zip)](https://github.com/stegidi/barstats-releases/releases/latest/download/BarStats.zip)**

#### 1. Trascina l'app
Scarica il file zip qui sopra, aprilo ed estrai **`BarStats.app`**. Poi **trascinala nella cartella Applicazioni** del tuo Mac.

#### 2. Il primo avvio (Perché macOS mostra un avviso?)
Poiché ho sviluppato questa app per me e per voi amici, non pago ad Apple i 99$ all'anno per la licenza commerciale di "sviluppatore identificato".

Per questo motivo, la primissima volta che provi ad aprire l'app, macOS ti mostrerà un messaggio di sicurezza dicendo che *«non è possibile verificare lo sviluppatore»*.

**Niente paura! Ci vogliono 5 secondi e va fatto SOLO la prima volta:**

* **Modo rapido con il mouse:**
  1. Apri il **Finder** e vai nella cartella **Applicazioni**.
  2. Fai **clic destro** (oppure tieni premuto il tasto `Control` e clicca) su **BarStats**.
  3. Clicca su **Apri** dal menu a tendina.
  4. Nella finestrella di avviso che si apre, clicca sul pulsante **Apri**.

* *(Oppure, se usi il Terminale, apri il Terminale, incolla questo comando e premi Invio:)*
  ```bash
  xattr -cr /Applications/BarStats.app
  ```

#### 3. Avvio automatico (facoltativo)
Vuoi che BarStats parta da solo ogni volta che accendi il Mac? Clicca sull'icona nella barra dei menu e apri **Generali ▸** e attiva **«Apri al login»**. Fatto!

---

### 🦀 Il granchietto di Claude Code (facoltativo)

Se usi **Claude Code** nel Terminale, BarStats può mostrarti a colpo d'occhio cosa sta facendo:
* 🔨 **sta lavorando**,
* ✋ **aspetta un tuo permesso**,
* ✅ **ha finito**.

Nel menu trovi anche l'elenco di tutte le sessioni aperte, ognuna con il suo stato.

**Come attivarlo:**
1. Assicurati che **BarStats sia nella cartella Applicazioni** (non avviarla dalla cartella Download!).
2. Clicca sull'icona nella barra dei menu, apri **Claude Code ▸** e attiva **«Collega a Claude Code»**.

*(Dietro le quinte l'app aggiunge qualche "hook" al file `~/.claude/settings.json`, così Claude Code può avvisarla quando cambia stato. Prima di toccarlo ne fa sempre una **copia di backup**. Se disattivi la levetta, gli hook vengono rimossi e il file torna com'era.)*

---

### 🔄 E per i prossimi aggiornamenti?

**Non dovrai più fare nulla di tutto questo!**

BarStats ha il sistema di aggiornamento automatico integrato:
* Quando pubblicherò nuove funzioni o correzioni, l'app se ne accorgerà da sola e ti mostrerà un avviso.
* Con un clic scaricherà la nuova versione e si riavvierà da sola.
* Puoi anche controllare manualmente in qualsiasi momento cliccando sull'icona di BarStats nella barra dei menu in alto e scegliendo **Generali ▸ «Controlla aggiornamenti…»**.
* Tutti i futuri aggiornamenti saranno già considerati sicuri dal tuo Mac e non mostreranno più alcun avviso di Gatekeeper!

---

### 🗑️ Come disinstallarla

1. Se avevi attivato il granchietto, **prima** disattiva **Claude Code ▸ «Collega a Claude Code»** dal menu (così gli hook vengono tolti da `~/.claude/settings.json`).
2. Chiudi BarStats con **«Esci da BarStats»** in fondo al menu.
3. Trascina **`BarStats.app`** dalla cartella Applicazioni nel **Cestino**. Fine!

---

<details>
<summary>🇬🇧 English version (Click to expand)</summary>

### Welcome to BarStats 📊

I built **BarStats** (formerly *TempBar*) to keep an eye on my Mac right from the menu bar.

* Show up to **3 live metrics** in the menu bar: **temperature, CPU, RAM, GPU, disk, network and fans**.
* Click the icon to see **every metric at once** and pick which ones to pin from the tile grid.
* No password or `sudo` needed, and it pauses while the screen is off.
* **Optional for Claude Code users:** a pixel crab 🦀 shows your sessions' status (working / waiting for permission / done), with a per-session list in the menu.

#### 🚀 First-Time Installation

👉 **[Download the latest release (.zip)](https://github.com/stegidi/barstats-releases/releases/latest/download/BarStats.zip)**

1. Extract the zip and **drag `BarStats.app` into your Applications folder**.
2. **First-launch macOS prompt**:
   Because I don't pay Apple $99/year for a developer certificate, macOS will say *“cannot verify developer”* on first open.
   * **Easy fix**: Right-click (or Control-click) `BarStats.app` in `/Applications` $\to$ click **Open** $\to$ click **Open**.
   * *(Or in Terminal: `xattr -cr /Applications/BarStats.app`)*.
3. **Launch at login** (optional): turn on **Generali ▸ “Apri al login”** in the menu.

#### 🦀 Claude Code crab (optional)
With the app in `/Applications`, turn on **Claude Code ▸ “Collega a Claude Code”** in the menu. It adds hooks to `~/.claude/settings.json` (after making a backup); turning it off removes them.

#### 🔄 Future Updates
Automatic! Whenever I publish an update, the app notifies you, updates itself, and restarts seamlessly. You can also click **Generali ▸ “Controlla aggiornamenti…”** in the menu bar at any time.

#### 🗑️ Uninstall
Turn off **“Collega a Claude Code”** first (if enabled), quit the app, then drag `BarStats.app` to the Trash.

</details>
