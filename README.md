<div align="center">

<img src="docs/flowtv-icon.png" alt="FlowTV" width="140">

# FlowTV – OpenWebif-IPTV

**Windows client for Enigma2 receivers over OpenWebif**

[Deutsch](#deutsch) · [English](#english) · [Download](../../releases/latest)

</div>

---

## English

FlowTV turns a Windows PC into a second TV set for an Enigma2 receiver. It talks
to the box over **OpenWebif**, shows your own channel lists with picons, the
programme guide, live TV, timers and recordings – and it never shows a black
screen while switching channels.

### What it does

- **Channel lists with picons**, straight from your box. Favourites and a
  „recently watched" list live on the PC, so they are there even when the box is
  off.
- **Live TV** through LibVLC, with the standard port and the stream relay port
  for encrypted channels; if one does not answer, the other is used.
- **Programme guide** with a grid, a detail card and a search over all channels.
- **Timers**: record or just switch over at the start of a programme, with tuner
  conflict detection – it will not start something that would break a running
  recording.
- **Recordings**: watch with resume, download over FTP/SFTP/HTTP with a queue,
  rename, move, delete.
- **Box control**: standby, restart, shutdown, a terminal with prepared commands
  and a backup of the box settings.
- **Dark, TiviMate-like interface**, German and English, adjustable font size and
  freely assignable keys.

### Download and start

1. Get the latest `FlowTV-<version>-win-x64.zip` from the
   [Releases page](../../releases/latest).
2. Unpack it to any folder – for example `C:\Programme\FlowTV`. **Do not run it
   from inside the ZIP.**
3. Start `FlowTV.exe`.

**Windows will warn you on the first start** („Windows protected your PC"). The
program is not code-signed – a certificate costs money that this project does not
have. Click **More info** and then **Run anyway**. If you would rather not, that
is a legitimate decision; the warning says nothing about what the program does.

**Windows Firewall** will ask for network access on the first start. FlowTV needs
it for **private networks** – that is where your receiver is.

### What you need

**On the PC – nothing to install beforehand:**

- 64-bit Windows 10 or 11.
- No .NET: the runtime is inside the folder.
- No VLC: LibVLC ships as its own DLLs in the `libvlc` subfolder.
- No Visual C++ redistributable.

**On the receiver:**

- **OpenWebif must be running** and reachable – without it, nothing works.
- **SSH** (Dropbear or OpenSSH) for the terminal and the settings backup.
- **FTP or SFTP** for downloading recordings.
- For encrypted channels over a stream relay: the relay service and its list at
  `/etc/enigma2/whitelist_streamrelay`.

Whatever is missing simply stays greyed out and says why – the rest keeps
working.

### First start

A short wizard searches the local network for boxes, asks for the login and
detects what your box can do. Everything it finds can be overridden by hand, and
every value shows where it came from: default, detected or set by you.

### Tested on one box only – please read this

This project has one developer and one receiver. **Everything you see was tested
on a GigaBlue UHD TRIO 4K with openATV 7.6 and OpenWebif 2.4.**

- **Receivers with several tuners could not be tested.** The most delicate part
  sits exactly there: counting tuners per reception type, comparing
  transponders, and protecting a running recording. That logic is covered by
  automated tests and written defensively, but nobody has watched it run on real
  hardware with more than one tuner.
- **Other images** (VTi, OpenPLi, PurE2 …) are untested. The app parses
  defensively and greys out what a box cannot do – that is what it is built for,
  but it is not proven.

**Bug reports are very welcome, especially from other boxes.** Please open an
[issue](../../issues) and attach the **diagnostics export** (Settings →
Diagnostics): it anonymises credentials and contains exactly the answers of your
box that are needed to understand the problem.

And the honest part: a bug that only happens on a box that is not standing here
may not be reproducible, and then it cannot be fixed with certainty. Please
report it anyway – several reports about the same box make a pattern.

### Support the project

FlowTV is made in spare time and is free for you. If you would like to support
it, there is a **coffee fund**:

- [Ko-fi](https://ko-fi.com/the_flow)
- [Revolut](https://revolut.me/the_flow)

Crypto addresses (BTC, ETH, SOL, XRP) are inside the app under **Buy me a
coffee**, with copy buttons and QR codes – so there is only one place where they
are kept, and it cannot go out of sync.

Feedback is worth just as much as money: bugs and ideas are what the next
version is made of.

### License

The program code is **proprietary** – see [LICENSE.txt](LICENSE.txt). It is not
open source, and this repository contains no source code.

The app ships third-party software; name, version, license and project page of
every component are listed in
[THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt), the full license texts are in
[licenses](licenses). In particular **LibVLC is used under LGPL-2.1-or-later**:
its files are separate, replaceable libraries in the `libvlc` subfolder next to
the program – neither statically linked nor bundled – and can be exchanged for
another build. Sources: <https://code.videolan.org/videolan/vlc>

FlowTV ships **no channel lists, picons or programme data**. Everything you see
comes from your own receiver.

### Not affiliated

FlowTV is an independent work. It is **not officially affiliated with the
OpenWebif project, with VideoLAN, or with any receiver manufacturer**, and is
neither endorsed nor reviewed by them. Names and trademarks mentioned belong to
their respective owners and are used only to describe the interface.

---

## Deutsch

FlowTV macht aus einem Windows-PC einen zweiten Fernseher für einen
Enigma2-Receiver. Es spricht über **OpenWebif** mit der Box, zeigt deine eigenen
Senderlisten mit Picons, die Programmzeitschrift, Live-TV, Timer und Aufnahmen –
und beim Umschalten gibt es nie ein schwarzes Bild.

### Was es kann

- **Senderlisten mit Picons**, direkt von der Box. Favoriten und „zuletzt
  gesehen" liegen auf dem PC und sind auch da, wenn die Box aus ist.
- **Live-TV** über LibVLC, mit Standardport und Stream-Relay-Port für
  verschlüsselte Sender; antwortet der eine nicht, wird der andere genommen.
- **TV-Guide** mit Raster, Detailkarte und Suche über alle Sender.
- **Timer**: aufnehmen oder zur Sendezeit nur umschalten, mit Erkennung von
  Tuner-Konflikten – es wird nichts gestartet, was eine laufende Aufnahme
  abbrechen würde.
- **Aufnahmen**: ansehen mit Fortsetzen, herunterladen über FTP/SFTP/HTTP mit
  Warteschlange, umbenennen, verschieben, löschen.
- **Box-Steuerung**: Standby, Neustart, Ausschalten, ein Terminal mit
  vorbereiteten Befehlen und eine Sicherung der Box-Einstellungen.
- **Dunkle, TiviMate-ähnliche Oberfläche**, Deutsch und Englisch, einstellbare
  Schriftgröße und frei belegbare Tasten.

### Herunterladen und starten

1. Die neueste `FlowTV-<Version>-win-x64.zip` von der
   [Releases-Seite](../../releases/latest) holen.
2. In einen beliebigen Ordner **entpacken** – zum Beispiel
   `C:\Programme\FlowTV`. **Nicht aus der ZIP heraus starten.**
3. `FlowTV.exe` starten.

**Windows warnt beim ersten Start** („Der Computer wurde durch Windows
geschützt"). Das Programm ist nicht signiert – ein Zertifikat kostet Geld, das
dieses Projekt nicht hat. Auf **Weitere Informationen** und dann **Trotzdem
ausführen** klicken. Wer das nicht möchte, hat gute Gründe; die Warnung sagt
nichts darüber aus, was das Programm tut.

**Die Windows-Firewall** fragt beim ersten Start nach Netzwerkzugriff. FlowTV
braucht ihn für **private Netzwerke** – dort steht dein Receiver.

### Was du brauchst

**Auf dem PC – nichts vorinstallieren:**

- 64-Bit-Windows 10 oder 11.
- Kein .NET: Die Laufzeit liegt im Ordner.
- Kein VLC: LibVLC liegt als eigene DLL-Sammlung im Unterordner `libvlc`.
- Kein Visual C++ Redistributable.

**Auf der Box:**

- **OpenWebif muss laufen** und erreichbar sein – ohne das geht gar nichts.
- **SSH** (Dropbear oder OpenSSH) für das Terminal und die Einstellungssicherung.
- **FTP oder SFTP** zum Herunterladen von Aufnahmen.
- Für verschlüsselte Sender über ein Stream-Relay: der Relay-Dienst und seine
  Liste unter `/etc/enigma2/whitelist_streamrelay`.

Was fehlt, bleibt ausgegraut und erklärt sich – der Rest läuft weiter.

### Der erste Start

Ein kurzer Assistent sucht im Netzwerk nach Boxen, fragt nach der Anmeldung und
erkennt, was deine Box kann. Alles Erkannte lässt sich von Hand überschreiben,
und bei jedem Wert steht, woher er kommt: Standard, erkannt oder selbst gesetzt.

### Geprüft nur an einer Box – bitte lesen

Hinter diesem Projekt stehen ein Entwickler und ein Receiver. **Alles, was du
hier siehst, ist an einer GigaBlue UHD TRIO 4K mit openATV 7.6 und OpenWebif 2.4
geprüft worden.**

- **Receiver mit mehreren Tunern konnten nicht geprüft werden.** Genau dort
  sitzt der empfindlichste Teil: die Tunerzählung nach Empfangsart, der
  Transpondervergleich und der Schutz einer laufenden Aufnahme. Diese Logik ist
  mit automatischen Tests abgedeckt und defensiv gebaut, aber an echter Hardware
  mit mehreren Tunern hat sie niemand laufen sehen.
- **Andere Images** (VTi, OpenPLi, PurE2 …) sind ungeprüft. Die App parst
  defensiv und graut aus, was eine Box nicht kann – dafür ist sie gebaut,
  bewiesen ist es nicht.

**Fehlermeldungen sind ausdrücklich willkommen, gerade von anderen Boxen.**
Bitte ein [Issue](../../issues) aufmachen und den **Diagnose-Export** anhängen
(Einstellungen → Diagnose): Er anonymisiert Zugangsdaten und enthält genau die
Antworten deiner Box, die zum Verstehen nötig sind.

Und der ehrliche Teil: Ein Fehler, der nur an einer Box auftritt, die hier nicht
steht, lässt sich womöglich nicht nachstellen und damit nicht sicher beheben.
Melde ihn trotzdem – aus mehreren Meldungen zur selben Box wird ein Muster.

### Das Projekt unterstützen

FlowTV entsteht in der Freizeit und ist für dich kostenlos. Wer es unterstützen
möchte, findet hier die **Kaffeekasse**:

- [Ko-fi](https://ko-fi.com/the_flow)
- [Revolut](https://revolut.me/the_flow)

Die Krypto-Adressen (BTC, ETH, SOL, XRP) stehen **in der App** unter **Kaffee
spendieren**, mit Kopierknöpfen und QR-Codes – so gibt es für sie nur eine
Stelle, und die kann nicht auseinanderlaufen.

Eine Rückmeldung ist genauso viel wert wie Geld: Fehler und Ideen sind das,
woraus die nächste Fassung entsteht.

### Lizenz

Der Programmcode ist **proprietär** – siehe [LICENSE.txt](LICENSE.txt). Er steht
nicht unter einer Open-Source-Lizenz, und dieses Repository enthält keinen
Quelltext.

Die App liefert Software Dritter mit; Name, Fassung, Lizenz und Projektseite
jedes Bestandteils stehen in
[THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt), die vollständigen
Lizenztexte im Ordner [licenses](licenses). Insbesondere wird **LibVLC unter der
LGPL-2.1-or-later** verwendet: Die Dateien liegen als eigene, austauschbare
Bibliotheken im Unterordner `libvlc` neben dem Programm – weder statisch
eingebunden noch zusammengepackt – und lassen sich gegen eine andere Fassung
tauschen. Quelltexte: <https://code.videolan.org/videolan/vlc>

FlowTV liefert **keine Senderlisten, Picons oder Programmdaten** mit. Alles, was
zu sehen ist, kommt vom Receiver des Nutzers.

### Keine Verbindung zu Dritten

FlowTV ist ein eigenständiges Werk. Es ist **nicht offiziell verbunden mit dem
OpenWebif-Projekt, mit VideoLAN oder mit Herstellern von Receivern** und wird
von diesen weder unterstützt noch geprüft. Genannte Namen und Marken gehören
ihren jeweiligen Inhabern und werden nur zur Beschreibung der Schnittstelle
verwendet.
