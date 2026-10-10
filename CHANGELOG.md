# Änderungen / Changelog

Alle spürbaren Änderungen an FlowTV, neueste zuerst.
All notable changes to FlowTV, newest first.

## 2.4.0

Sicherung wie im Menü der Box, Einrichtung und Mac verbessert. /
Backup like the receiver menu, setup and Mac improved.

**Deutsch**

- **Neu: Einstellungssicherung wie im Menü von openATV.** Vorausgewählt ist,
  was openATV selbst sichert – Senderlisten, Timer, Einstellungen,
  Cam-Konfiguration, Netzwerk, Skin-Anpassungen und Paketquellen. In einem
  Box-Browser kreuzt du Ordner und einzelne Dateien beliebig tief dazu oder
  nimmst sie heraus. Gespeichert wird im Format der Box
  (`backup_<Image>_<Box>/enigma2settingsbackup.tar.gz`) samt Liste deiner
  Plugins: Ordner auf einen USB-Stick kopieren, und die Box findet die
  Sicherung beim Wiederherstellen. Eine ältere Sicherung im selben Ordner
  bekommt das Datum vorn dran. Benutzerdateien und Programme werden nie
  gesichert – sie passen nach einem Wechsel der Image-Version nicht mehr.
- **Vollsicherung:** Einstellungssicherungen werden nicht mehr fälschlich als
  Vollsicherung angeboten.
- **Behoben: FlowTV fror beim Umschalten ein** – am Mac bis zu zwei Minuten,
  beim Löschen aller Daten ganz. Das Anhalten des alten Senders läuft jetzt im
  Hintergrund.
- **Einrichtung:** „Weiter“ erst, wenn eine Box gewählt oder eingetragen ist;
  bei „Kein Dateizugriff“ steht jetzt der Grund dabei; die Picon-Prüfung ist
  nicht mehr grundlos gelb.
- **Einstellungen:** „Dateizugriff“ steht direkt unter „Streaming“.
- **Terminal: Markieren über mehrere Zeilen.** Mit gedrückter Maustaste lässt
  sich beliebig viel Ausgabe markieren. Kopieren mit Strg+C (Mac: Cmd+C) oder
  Rechtsklick → „Kopieren“, Strg+A markiert alles.
- **Update-Hinweis:** Wer eine Testversion hat, bekommt die fertige Version mit
  derselben Nummer angeboten.
- **Mac:** FlowTV kommt ins Heimnetz („Lokales Netzwerk“), echtes Vollbild.
- **Diagnose-Export und Protokoll:** Versionsnummern bleiben lesbar; schlägt
  ein Verbindungstest oder die Suche nach der Box fehl, steht der Grund im
  Protokoll.

**English**

- **New: settings backup like the openATV menu.** Preselected is what openATV
  backs up itself – channel lists, timers, settings, cam configuration,
  network, skin customisations and package feeds. In a box browser you tick
  further folders and single files at any depth or leave some out. It is
  saved in the receiver’s own format
  (`backup_<image>_<box>/enigma2settingsbackup.tar.gz`) including the list of
  your plugins: copy the folder to a USB stick and the box finds the backup
  when restoring. An older backup in the same folder gets the date in front.
  User files and programs are never backed up – they no longer fit after a
  change of image version.
- **Full backup:** settings backups are no longer offered as a full backup.
- **Fixed: FlowTV froze when switching channels** – on the Mac for up to two
  minutes, completely when deleting all data. Stopping the old channel now
  runs in the background.
- **Setup:** “Next” only once a receiver is chosen or entered; “No file
  access” now tells the reason; the picon check is no longer yellow for no
  reason.
- **Settings:** “File access” is now right below “Streaming”.
- **Terminal: select across lines.** Hold the mouse button to select as much
  output as you like. Copy with Ctrl+C (Mac: Cmd+C) or right-click → “Copy”,
  Ctrl+A selects everything.
- **Update notice:** test versions are offered the final version with the same
  number.
- **Mac:** FlowTV reaches the home network (“Local Network”), real full
  screen.
- **Diagnostics export and log:** version numbers stay readable; when a
  connection test or the receiver search fails, the reason is in the log.

## 2.3.2

Untertitel sind wieder ab Werk aus. / Subtitles are off by default again.

**Deutsch**

- **Behoben: Untertitel liefen von selbst** – bei Sendern mit Untertiteln oft
  „Deutsch für Hörgeschädigte“, obwohl „Untertitel anzeigen“ (Einstellungen →
  Wiedergabe) ab Werk aus steht. Jetzt bleiben sie aus, bis du sie bei einem
  Sender einschaltest (das merkt sich FlowTV je Sender) oder den Schalter
  anmachst.

**English**

- **Fixed: subtitles switched on by themselves** – on channels with subtitles
  often “German for the hearing impaired”, although “Show subtitles”
  (Settings → Playback) is off by default. Now they stay off until you switch
  them on for a channel (FlowTV remembers that per channel) or turn the switch
  on.

## 2.3.1

Behebungen beim Beenden und beim Löschen aller Daten. /
Fixes for closing FlowTV and for deleting all data.

**Deutsch**

- **Behoben: FlowTV konnte nach dem Schließen ohne Fenster weiterlaufen**
  (im Task-Manager sichtbar) und hielt seinen Ordner fest – vor allem nach
  „Alle gespeicherten Daten löschen“. Ist das Hauptfenster zu, beendet sich
  FlowTV jetzt immer.
- **Behoben: „Cannot re-show a closed window“**, wenn FlowTV gestartet wurde,
  während es sich gerade beendete. Der neue Start wartet jetzt, bis das alte
  FlowTV zu ist, und öffnet sich dann.
- **„Alle gespeicherten Daten löschen“ zeigt, dass gelöscht wird**, und
  FlowTV schließt sich erst, wenn wirklich alles weg ist – vorher blieb die
  Programmzeitschrift liegen. Klappt es nicht ganz, steht da, was übrig ist,
  mit dem Knopf „FlowTV schließen“.

**English**

- **Fixed: FlowTV could keep running without a window after closing**
  (visible in Task Manager) and kept its folder locked – mostly after
  “Delete all saved data”. Once the main window is closed, FlowTV now always
  exits.
- **Fixed: “Cannot re-show a closed window”** when FlowTV was started while it
  was still closing. The new start now waits until the old FlowTV has ended and
  then opens.
- **“Delete all saved data” shows that it is deleting**, and FlowTV only closes
  once everything is really gone – before, the programme guide was left
  behind. If not everything can be deleted, it says what is left and offers
  “Close FlowTV”.

## 2.3.0

Mehrere Boxen, Daten wohin du willst, Radio – und ein besserer TV-Guide. /
Several boxes, data wherever you like, radio – and a better TV guide.

**Deutsch**

- **Neu: Box wechseln unten links.** Mit mehreren Boxen (Profilen) ist die
  Zeile mit Name und Adresse unten links ein Knopf: Klick, Box wählen, fertig.
  Senderliste, TV-Guide, Timer und Aufnahmen kommen dann von der neuen Box.
- **Neu: Auf eine andere Box ausweichen.** Je Box lassen sich Ersatz-Boxen
  anhaken (Einstellungen → „Ausweichen auf andere Box“, ab Werk aus).
  Antwortet die Box nicht – etwa im Deep-Standby – oder belegen Aufnahmen alle
  Tuner, bietet FlowTV die erste erreichbare Ersatz-Box an. Ab Werk mit
  Rückfrage.
- **Neu: Profile umbenennen** – Zeile „Profilname“ ganz oben unter
  Einstellungen → Verbindung.
- **Neu: Daten neben dem Programm (portabel).** Liegt neben FlowTV ein Ordner
  `FlowTV-Data`, speichert FlowTV alles dort statt unter dem Benutzerprofil.
  Einstellungen → Daten auf dem PC → „Daten neben das Programm verlegen“ zieht
  um. Windows und Linux.
- **Neu: Beim allerersten Start fragt FlowTV, wo die Daten liegen sollen** –
  neben dem Programm (empfohlen), unter dem Benutzerprofil oder in einem
  eigenen Ordner. Wer FlowTV schon benutzt, wird nicht gefragt. Windows und
  Linux.
- **Neu: Schalter „Radio“ neben „Bouquets“** – Radio-Bouquets direkt in der
  Senderliste ein- und ausblenden, unter den TV-Bouquets mit einer feinen Linie.
- **TV-Guide füllt die Breite** und zeigt auf breiten Bildschirmen mehr Zeit;
  neben dem Blättern gibt es jetzt eine Auswahl „Heute, Morgen, …“.
- **Aufnahmen: Papierkorb und Systemordner ausblenden** (`trashcan`,
  `$RECYCLE.BIN`, `lost+found`), ab Werk an.
- **Behoben: Radiosender blieben bei „Der Sender wird geladen …“ stehen**, obwohl
  Musik lief, und FlowTV versuchte einen anderen Port. Jetzt zählt der Ton; im
  Player stehen Picon, Name und „Radio – nur Ton“.
- **Behoben: Nach dem ersten Einrichten stand „Noch keine Box eingerichtet.“**
  – die Senderliste kommt jetzt von selbst.
- **Behoben: Nach einem Boxwechsel blieben Senderliste und TV-Guide der alten
  Box stehen.**

**English**

- **New: switch boxes at the bottom left.** With several boxes (profiles) the
  line with name and address at the bottom left is a button: click, pick a box,
  done. Channel list, TV guide, timers and recordings then come from the new box.
- **New: fall back to another box.** Per box you can tick spare boxes
  (Settings → “Fall back to another box”, off by default). If the box does not
  answer – say, in deep standby – or recordings use all tuners, FlowTV offers
  the first spare box that answers. Asks first by default.
- **New: rename profiles** – “Profile name” at the top of Settings → Connection.
- **New: data next to the program (portable).** If there is a folder
  `FlowTV-Data` next to FlowTV, everything is stored there instead of in the
  user profile. Settings → Data on this PC → “Move data next to the program”
  moves it. Windows and Linux.
- **New: on the very first start FlowTV asks where to keep its data** – next to
  the program (recommended), in the user profile or in a folder of your own.
  Existing users are not asked. Windows and Linux.
- **New: “Radio” switch next to “Bouquets”** – show or hide radio bouquets right
  in the channel list, below the TV bouquets behind a thin line.
- **The TV guide fills the width** and shows more time on wide screens; next to
  the arrows there is now a “Today, Tomorrow, …” choice.
- **Recordings: hide recycle bin and system folders** (`trashcan`,
  `$RECYCLE.BIN`, `lost+found`), on by default.
- **Fixed: radio channels stayed at “Loading the channel …”** although music was
  playing, and FlowTV tried another port. Now the sound counts; the player shows
  picon, name and “Radio – audio only”.
- **Fixed: after the first setup it said “No box set up yet.”** – the channel
  list now loads by itself.
- **Fixed: after switching boxes, channel list and TV guide of the old box
  stayed.**

## 2.2.0

Was läuft auf der Box – und eine Rückfrage, bevor FlowTV den Fernseher stört. /
What's on the box – and a question before FlowTV disturbs the TV.

**Deutsch**

- **Neu: Leiste „Was läuft auf der Box“** unten im Fenster, auf jeder Seite:
  was der Fernseher gerade zeigt (Sender mit Sendung, oder welche Aufnahme
  abgespielt wird), welche Aufnahmen laufen und wer Streams bekommt – mit
  Tuner, wenn die Box ihn nennt. Die Zeichen pulsieren weiß-rot, damit man sie
  bemerkt. Abschaltbar unter Einstellungen → Oberfläche.
- **Neu: Rückfrage vor dem Umschalten.** Läuft am Fernseher gerade etwas, das
  FlowTV nicht selbst eingestellt hat – etwa eine Aufnahme, die jemand
  ansieht –, fragt FlowTV, bevor es die Box umschaltet. „Abbrechen“ lässt den
  Fernseher in Ruhe. Abschaltbar unter Einstellungen → Erst umschalten.
- **Boxen mit mehreren Tunern:** Freie Tuner werden je Empfangsart gezählt
  (Sat, Kabel, Antenne; ein Kombi-Tuner nur für eines zugleich), und vor dem
  Ansehen fragt FlowTV die Box, welche Tuner Fernsehbild, Aufnahmen und Streams
  gerade belegen. Gilt auch für den Aufnahmeschutz und die Timer-Konflikte.
  **An Boxen mit mehreren Sat-Tunern noch ungetestet** – Rückmeldungen erwünscht.
- **Neu: Bild bei Aufnahmen.** Schickt die Box zu einer Aufnahme keinen
  Sendernamen, steht statt „?“ ein Platzhalterbild davor. Wer mag, nimmt es für
  alle Aufnahmen (Einstellungen → Aufnahmen → „Bild bei Aufnahmen“).
- **Nach neuen Versionen wird jetzt bei jedem Start gefragt** und, solange
  FlowTV läuft, um 8, 12 und 18 Uhr. Der Punkt an „Über“ pulsiert gelb-orange.
- **„Unterordner einbeziehen“ findet Aufnahmen in allen Unterordnern**, egal
  wie tief. Die Einstellung „Maximale Tiefe“ entfällt.
- **Einstellungen aufgeräumt:** „Erkannte Box-Fähigkeiten“ steht unter
  „Verbindung“, „Zusätzliche Pfade“ unter „Aufnahmepfad auf der Box“.
- **Windows: Das Fenster „FlowTV startet …“ kommt beim ersten Start sofort**
  (nach unter einer Sekunde statt erst kurz vor dem Hauptfenster).

**English**

- **New: “What's on the box” bar** at the bottom of the window, on every page:
  what the box is showing on the TV (channel and programme, or which recording
  is playing), which recordings are running and who gets streams – with the
  tuner when the box names it. The symbols pulse white and red so you notice
  them. Can be switched off under Settings → User interface.
- **New: a question before switching.** If something the TV is showing was not
  set by FlowTV – say, a recording somebody is watching – FlowTV asks before it
  switches the box. “Cancel” leaves the TV alone. Can be switched off under
  Settings → Switch first.
- **Boxes with several tuners:** free tuners are counted per reception type
  (satellite, cable, terrestrial; a combo tuner only for one at a time), and
  before watching FlowTV asks the box which tuners are busy with the TV picture,
  recordings and streams. This also applies to the recording protection and the
  timer conflicts. **Not yet tested on boxes with several satellite tuners** –
  feedback welcome.
- **New: image for recordings.** If the box sends no channel name for a
  recording, a placeholder image appears instead of “?”. You can also use it for
  all recordings (Settings → Recordings → “Image for recordings”).
- **New versions are now checked at every start** and, while FlowTV is running,
  at 8 am, 12 pm and 6 pm. The dot at “About” pulses yellow and orange.
- **“Include subfolders” finds recordings in all subfolders**, however deep.
  The “Maximum depth” setting is gone.
- **Settings tidied up:** “Detected box capabilities” sits under “Connection”,
  “Additional paths” under “Recording path on the box”.
- **Windows: the “FlowTV is starting …” window appears right away** on the
  first start (in under a second instead of just before the main window).

## 2.1.1

Sicherer Start: FlowTV läuft nur noch einmal. /
Safer start: FlowTV only runs once.

**Deutsch**

- **FlowTV läuft nur noch einmal.** Ein zweiter Start öffnet kein zweites
  Fenster mehr, sondern holt das offene nach vorn. Zwei gleichzeitige FlowTV
  konnten sich gegenseitig Einstellungen überschreiben.
- **Beim ersten Start nach dem Entpacken** zeigt FlowTV sofort ein kleines
  Fenster „FlowTV startet …“. Windows prüft dann alle neuen Dateien einmal, und
  bis zum Hauptfenster kann es etwas dauern – so ist klar, dass es läuft.

**English**

- **FlowTV only runs once.** Starting it again no longer opens a second window
  but brings the open one to the front. Two FlowTV at the same time could
  overwrite each other's settings.
- **On the first start after unpacking** FlowTV shows a small “FlowTV is
  starting …” window right away. Windows checks all new files once, and the
  main window can take a while – now it is clear that it is running.

## 2.1.0

Hinweis auf neue Versionen, schnellerer Start, aufgeräumtes Vollbild. /
Notice of new versions, faster start, a tidier fullscreen bar.

**Deutsch**

- **Neu: Hinweis auf neue Versionen.** FlowTV sieht einmal am Tag bei GitHub
  nach, ob es eine neuere Version für dein System gibt. Dann bekommt „Über“
  einen farbigen Punkt, und dort führt ein Knopf zur Release-Seite. Kein Popup,
  kein automatischer Download; abschaltbar unter Einstellungen → Oberfläche.
- **Neu: Versionsgeschichte** auf der Seite „Über“, zum Aufklappen.
- **Neu: Eigener Timer aus der Senderliste.** Rechtsklick auf einen Sender →
  Timer → „Eigener Timer …“ – Zeiten frei wählbar, der Sender ist schon
  ausgewählt.
- **Schnellerer Start.** Die Senderliste ist sofort da. Solange die Wiedergabe
  vorbereitet wird, steht das im Bild, und ein gewählter Sender startet danach
  von selbst. Unter Windows entfällt ab dem zweiten Start das lange Warten nach
  dem Hochfahren des PCs.
- **Aufnahmen wecken Box und Fernseher nicht mehr.** Je nach Box-Einstellung
  holte ein Aufnahme-Timer die Box aus dem Standby – und über HDMI-CEC den
  Fernseher gleich mit. FlowTV sagt der Box jetzt „nur aufnehmen“; einstellbar
  unter Einstellungen → Aufnahmen.
- **Vollbild: Bildschirm aus einer Liste wählen** (Bildschirm 1, 2 … mit
  Auflösung) statt reihum weiterzuschieben.
- **Vollbild: Tonspur und Untertitel in einem Knopf** mit Liste zum Anklicken.
- **Verständliche Tonspuren und Untertitel:** „Deutsch“, „Französisch“,
  „Deutsch · Hörfassung (Audiodeskription)“, „Deutsch · Dolby Digital“,
  „Deutsch · für Hörgeschädigte“ statt „Track 1 - [German]“. Die gewählte
  Tonspur wird je Sender wieder gemerkt. Videotext-Untertitel stehen nicht
  mehr zur Wahl – nur noch die gut lesbaren DVB-Untertitel.
- **Schmale Fenster:** Der Hinweis „Aufnahme läuft …“ und die Leisten bleiben
  lesbar – die Knöpfe rücken darunter oder zeigen nur ihr Symbol. Die
  Senderliste behält ihren Platz, die Bouquet-Spalte wird schmaler.

**English**

- **New: notice of new versions.** Once a day FlowTV checks GitHub for a newer
  version for your system. If there is one, “About” gets a coloured dot and a
  button to the release page. No pop-up, no automatic download; can be turned
  off under Settings → User interface.
- **New: version history** on the “About” page, to fold out.
- **New: custom timer from the channel list.** Right-click a channel → Timer →
  “Custom timer …” – free start and end, the channel already chosen.
- **Faster start.** The channel list is there at once. While playback is being
  prepared the picture says so, and a channel chosen meanwhile starts by itself.
  On Windows the long wait after booting the PC is gone from the second start on.
- **Recordings no longer wake the box and the TV.** Depending on a box setting,
  a recording timer brought the box out of standby – and the TV along with it
  over HDMI-CEC. FlowTV now tells the box “record only”; adjustable under
  Settings → Recordings.
- **Fullscreen: choose the screen from a list** (screen 1, 2 … with resolution)
  instead of moving it on one by one.
- **Fullscreen: audio track and subtitles in one button** with a list.
- **Readable audio tracks and subtitles:** “German”, “French”, “German ·
  Audio description”, “German · Dolby Digital”, “German · for the hard of
  hearing” instead of “Track 1 - [German]”. The chosen audio track is
  remembered per channel again. Teletext subtitles are no longer offered –
  only the clearly readable DVB subtitles.
- **Narrow windows:** the “Recording …” notice and the bars stay readable – the
  buttons move below or show only their icon. The channel list keeps its
  room, the bouquet column gets narrower.

## 2.0.0

Neu gebaute Oberfläche und viele Verbesserungen aus dem Alltag. /
Rebuilt interface and many improvements from everyday use.

**Deutsch**

- **Neue Oberfläche.** FlowTV ist von Grund auf neu gebaut (Avalonia statt
  WPF). Aussehen und Bedienung bleiben vertraut; Einstellungen, Favoriten und
  Tastenbelegung aus 1.0 werden einfach übernommen.
- **Neu: Linux (Vorschau).** Dieselbe App als `linux-x64`. VLC kommt dort aus
  der Paketverwaltung (`sudo apt install vlc`). Geprüft unter Ubuntu 24.04 in
  WSL2 – siehe README.
- **Neu: Mac (Vorschau, ungetestet).** `FlowTV.app` als Intel-Build, auf
  Macs mit Apple-Chip über Rosetta 2. Auf einem echten Mac noch nicht geprüft –
  Rückmeldungen sehr willkommen.
- **Vollbild auf dem richtigen Bildschirm.** Das Vollbild ist jetzt ein eigenes
  Fenster: Es erscheint auf dem Bildschirm, auf dem FlowTV liegt, lässt sich mit
  „Anderer Bildschirm" weiterschieben und merkt sich die Wahl. Das Hauptfenster
  bleibt daneben bedienbar.
- **Aufnahmen laufen beim Seitenwechsel weiter.** Wer während einer Aufnahme in
  den TV-Guide oder zu den Timern wechselt, sieht weiter. Beendet wird sie erst
  mit „Wiedergabe beenden", „Zum Fernsehen zurück" oder einem neuen Sender – die
  Stelle wird gemerkt.
- **Springen in Aufnahmen**: 30 Sekunden vor und zurück, jetzt gleichmäßig und
  zuverlässig.
- **Tonspur**: Vorausgewählt ist die gewöhnliche Spur in deiner Sprache -
  Hörfassungen und „clean audio" kommen danach. Gilt jetzt auch für Aufnahmen.
- **Herunterladen** mit richtigem Speichern-Dialog: Der Name der Aufnahme ist
  schon eingetragen.
- **Timer ohne eigene Beschreibung** bekommen die ersten Zeilen aus dem EPG statt
  nur der Kurzzeile („Fernsehfilm Deutschland 2019").
- **Tasten wirken auch mit Fokus in der Senderliste** (F, M, S, Z …); Pfeil
  links/rechts schaltet auch von dort um.
- **Esc im Vollbild** schließt erst das Mini-EPG, dann das Vollbild.
- **Die Steuerleiste im Vollbild** verschwindet nicht mehr unter der Maus.
- **Einstellungen durchsuchen** findet in beiden Sprachen – „Sprache" findet auch
  die Einstellung, wenn die Oberfläche auf Englisch steht.
- **Titel mit „&" oder Apostroph** stehen im EPG richtig da.
- „Box aufwecken" steht im Vollbild nicht mehr direkt neben „Aufnehmen" – ein
  Klick zu viel weckte dort die Box und über HDMI-CEC den Fernseher gleich mit.

**English**

- **New interface.** FlowTV has been rebuilt from scratch (Avalonia instead of
  WPF). Look and handling stay familiar; settings, favourites and key bindings
  from 1.0 carry over.
- **New: Linux (preview).** The same app as `linux-x64`. VLC comes from the
  package manager there (`sudo apt install vlc`). Tested on Ubuntu 24.04 in
  WSL2 – see the README.
- **New: Mac (preview, untested).** `FlowTV.app` as an Intel build, on Apple
  silicon through Rosetta 2. Not yet checked on a real Mac – reports very
  welcome.
- **Fullscreen on the right screen.** Fullscreen is now a window of its own: it
  opens on the screen FlowTV is on, moves on with “Other screen” and remembers
  the choice. The main window stays usable next to it.
- **Recordings keep playing when you switch pages.** Watching a recording and
  opening the guide or the timers no longer stops it. It ends with “Stop
  playback”, “Back to TV” or a new channel – and the position is remembered.
- **Skipping in recordings**: 30 seconds forward and back, now even and reliable.
- **Audio track**: the regular track in your language is chosen first – audio
  description and “clean audio” come after. Now for recordings as well.
- **Downloads** with a proper save dialog, the recording's name already filled in.
- **Timers without a description of their own** get the first lines from the EPG
  instead of just the short line (“TV film Germany 2019”).
- **Keys work with the focus in the channel list** (F, M, S, Z …); left/right
  switch channels from there too.
- **Esc in fullscreen** closes the mini guide first, then fullscreen.
- **The fullscreen control bar** no longer disappears under the mouse.
- **Searching the settings** works in both languages.
- **Titles with “&” or an apostrophe** show correctly in the guide.
- “Wake the box” no longer sits right next to “Record” in fullscreen – one click
  too many woke the box there, and the TV along with it over HDMI-CEC.

## 1.0.0

Erste Veröffentlichung. / First public release.

**Deutsch**

- Senderlisten mit Picons, Favoriten und „zuletzt gesehen"
- Live-TV über LibVLC, Standard- und Stream-Relay-Port mit automatischem
  Ausweichen; beim Umschalten bleibt das letzte Bild stehen statt schwarz zu
  werden
- TV-Guide mit Raster, Detailkarte und Suche über alle Sender
- Timer zum Aufnehmen und zum Umschalten, mit Erkennung von Tuner-Konflikten
  und Schutz laufender Aufnahmen
- Aufnahmen ansehen mit Fortsetzen, herunterladen mit Warteschlange,
  umbenennen, verschieben, löschen
- Box-Steuerung: Standby, Neustart, Ausschalten, Terminal mit vorbereiteten
  Befehlen, Sicherung der Box-Einstellungen mit Auswahl, was mitgeht
- Einrichtungsassistent mit Suche im Netzwerk und Erkennung; jeder Wert zeigt,
  ob er Standard, erkannt oder selbst gesetzt ist
- Dunkle Oberfläche, Deutsch und Englisch, einstellbare Schriftgröße, frei
  belegbare Tasten
- Portabel: entpacken und starten, kein Installer, nichts vorzuinstallieren

**English**

- Channel lists with picons, favourites and a “recently watched” list
- Live TV through LibVLC, standard and stream relay port with automatic
  fallback; the last frame stays on screen while switching instead of going
  black
- Programme guide with grid, detail card and a search across all channels
- Timers for recording and for switching over, with tuner conflict detection
  and protection of running recordings
- Recordings with resume, download queue, rename, move, delete
- Box control: standby, restart, shutdown, terminal with prepared commands,
  backup of the box settings with a choice of what goes in
- Setup wizard with network search and detection; every value shows whether it
  is a default, detected or set by hand
- Dark interface, German and English, adjustable font size, freely assignable
  keys
- Portable: unpack and start, no installer, nothing to install beforehand
