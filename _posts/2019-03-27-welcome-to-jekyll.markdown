---
layout: post
title:  "Windows 10 SmartScreen ausschalten"
date:   2019-03-27 16:20:19 +0100
categories: windows hilfe
permalink: /windows-smartscreen-ausschalten
excerpt: Ach ja der liebe Computer. Manchmal kann er ärger bereiten, sodass ein glückliches Arbeiten schwer wird. Das kennen wir alle. Im Fall der Windows 10 Smartscreen ausschaltens, kennen wir aber die Lösung! Heute erklären wir es deshalb, Schritt für Schritt.
---

Ach ja der liebe Computer.

Manchmal kann er ärger bereiten, sodass ein glückliches Arbeiten schwer wird.

Das kennen wir alle. Im Fall der Windows 10 Smartscreen ausschaltens, kennen wir aber die Lösung!

Heute erklären wir es deshalb, Schritt für Schritt.

und mit Bildern ;)

Legen wir los.

Der Windows SmartScreen ist ein Anti-Malware-Filter, der Ihren PC vor verdächtigen Anwendungen und Malware schützt. Immer wenn Sie versuchen, eine nicht erkannte App zu installieren, erscheint die Warnmeldung SmartScreen, die den Benutzer über die Gefahr informiert. Neben dem Schutz des PCs schützt es auch die Privatsphäre des Benutzers.

Windows Smartscreen kann auch verhindern, dass Sie tatsächlich etwas Nützliches aus dem Internet herunterladen. So entfernen oder deaktivieren Sie den Windows Smartscreen-Filter in Windows 10.



Deaktivieren über die Sicherheitseinstellungen von Windows Defender
Sie können den Windows Smartscreen über die Windows-Sicherheitseinstellungen deaktivieren, indem Sie diesen drei einfachen Schritten folgen.

<h2>Schritt 1</h2>

<img src="/windows-sicherheitscenter-suche.png" alt="windows sicherheitscenter suchen">

<h2>Schritt 2</h2>

<img src="/sicherheitescenter.png" alt="windows sicherheitscenter apps">


Sobald das Windows Defender Security Centre geöffnet ist, suchen Sie nach Apps & Browser Control, das sich auf der linken Seite des Dialogfelds befindet.

<h2>Schritt 3</h2>

<img src="/smartscreen_ausschalten.png" alt="windows sicherheitscenter suchen">

Suchen Sie unter dem Apps & Browser Control nach Smartscreen für Microsoft Edge. Sie können dann zwischen Block, Warnung oder Aus umschalten. Toggling Block zeigt eine Warnmeldung an und verhindert, dass die nicht erkannte Anwendung ausgeführt wird. Warnung zeigt Ihnen eine Warnmeldung und gibt Ihnen die Möglichkeit, die nicht erkannte Anwendung zum Ausführen auszuwählen oder nicht.


<h1>Ausschalten Durch den Windows Registry Editor</h1>

Der Windows Registry Editor ist ein leistungsstarker Editor, mit dem Sie Änderungen an vielen Programmen auf dem PC vornehmen können. Stellen Sie aus diesem Grund sicher, dass Sie ein Backup erstellen oder einen Systemwiederherstellungspunkt erstellen,wenn etwas schief geht. Hier erfahren Sie, wie Sie Windows SmartScreen in acht einfachen Schritten deaktivieren können.

<h2>Schritt 1</h2>


Öffnen Sie die Windows-Registrierung, indem Sie die Windows-Taste + R drücken, um run zu öffnen und regedit einzugeben. Sie können auch mit der rechten Maustaste auf das Windows-Symbol klicken und Ausführen auswählen.

<h2>Schritt 2</h2>


Der Windows Registry Editor wird geöffnet. Fahren Sie fort, Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\System in den Pfad zu kopieren und einzufügen, wie durch das rote Kästchen in Ihrem Windows Registry Editor angezeigt. Drücken Sie Enter.



<h2>Schritt 3</h2>

<img src="/dword-erstellen.png" alt="Erstellen von dword value">


Klicken Sie mit der rechten Maustaste auf den weißen Bereich in der rechten Seitenleiste. Erstellen Sie dann einen neuen DWORD (32-Bit) Wert-Schlüssel.

<h2>Schritt 4</h2>

dword umbenennen
Umbenennen von DWORD
Fahren Sie fort, den DWORD-Schlüssel in EnableSmartScreen umzubenennen.

<h2>Schritt 5</h2>

Ändern des dword
Ändern des DWORTes
Doppelklicken Sie auf den neu erstellten Schlüssel EnableSmartScreen, um ihn zu bearbeiten. Geben Sie unter Wertdaten 0 zum Deaktivieren oder 1 zum Aktivieren ein.

<h2>Schritt 6</h2>

Erstellen des Zeichenkettenwertes
Erstellen des Zeichenkettenwertes
Klicken Sie mit der rechten Maustaste auf das gleiche rechte Seitenfenster, um einen neuen Zeichenkettenwert zu erstellen.

<h2>Schritt 7</h2>

<img src="/string_value_umbennen.png" alt="windows sicherheitscenter suchen">

Umbenennen des Zeichenkettenwertes
Umbenennen des Zeichenkettenwertes
Benennen Sie den neuen String Value ShellSmartScreenLevel um.

<h2>Schritt 8</h2>

Setzen des Zeichenkettenwertes
Einstellen des Wertes für die Zeichenkette
Doppelklicken Sie auf ShellSmartScreenLevel, um es zu bearbeiten. Unter Wertdaten können Sie Block, Warnung oder Aus eingeben. Aus deaktiviert die Warnmeldung, wenn eine nicht erkannte Anwendung ausgeführt wird.

<h1>Deaktivieren über den Editor für lokale Gruppenrichtlinien</h1>


Für Benutzer von Windows 10 Pro und Enterprises können Sie den Windows Smartscreen über den Local Group Policy Editor deaktivieren.

Drücken Sie die Tasten Windows + R oder geben Sie RUN in die Suche ein, indem Sie auf die Schaltfläche Search Lupe im Aufgabenmenü klicken.

<ul>
<li>Sobald RUN geöffnet ist, geben Sie gpedit.msc ein und klicken Sie auf OK.</li>

<li>Ein Editor für lokale Gruppenrichtlinien wird dann geöffnet.</li>

<li>Navigieren Sie zu Computerkonfiguration > Administrative Vorlagen > Windows-Komponenten > Datei-Explorer.</li>

<li>Wählen Sie Configure Windows Defender SmartScreen und doppelklicken Sie darauf, um die Einstellungen zu öffnen.</li>

<li>Aktivieren Sie in den Richtlinieneinstellungen das Optionsfeld Deaktiviert und klicken Sie auf OK.</li>

<li>Wählen Sie unter den Optionen "Warnung und Vermeidung von Bypass".</li>

<li>Schließen Sie den Editor für lokale Gruppenrichtlinien und starten Sie Ihren Computer neu, damit Änderungen wirksam werden.</li>
</ul>
