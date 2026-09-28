# Änderungen / Changelog

Alle spürbaren Änderungen an FlowTV, neueste zuerst.
All notable changes to FlowTV, newest first.

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
