---
layout: post
title:  "Windows 10 SmartScreen ausschalten"
date:   2019-03-27 16:20:19 +0100
categories: windows hilfe
permalink: /windows-smartscreen-ausschalten

---
Der Windows SmartScreen ist ein Anti-Malware-Filter, der Ihren PC vor verdächtigen Anwendungen und Malware schützt. Immer wenn Sie versuchen, eine nicht erkannte App zu installieren, erscheint die Warnmeldung SmartScreen, die den Benutzer über die Gefahr informiert. Neben dem Schutz des PCs schützt es auch die Privatsphäre des Benutzers.

Windows Smartscreen kann auch verhindern, dass Sie tatsächlich etwas Nützliches aus dem Internet herunterladen. So entfernen oder deaktivieren Sie den Windows Smartscreen-Filter in Windows 10.

Deaktivieren über die Sicherheitseinstellungen von Windows Defender
Sie können den Windows Smartscreen über die Windows-Sicherheitseinstellungen deaktivieren, indem Sie diesen drei einfachen Schritten folgen.

Schritt 1

Schritt 2

<img src="/windows-sicherheitscenter-suche.png" alt="windows sicherheitscenter suchen">

Sobald das Windows Defender Security Centre geöffnet ist, suchen Sie nach Apps & Browser Control, das sich auf der linken Seite des Dialogfelds befindet.

Schritt 3


Suchen Sie unter dem Apps & Browser Control nach Smartscreen für Microsoft Edge. Sie können dann zwischen Block, Warnung oder Aus umschalten. Toggling Block zeigt eine Warnmeldung an und verhindert, dass die nicht erkannte Anwendung ausgeführt wird. Warnung zeigt Ihnen eine Warnmeldung und gibt Ihnen die Möglichkeit, die nicht erkannte Anwendung zum Ausführen auszuwählen oder nicht.

Verwandt: Beste Laptop-Angebote vor dem Brand


Der Windows Registry Editor ist ein leistungsstarker Editor, mit dem Sie Änderungen an vielen Programmen auf dem PC vornehmen können. Stellen Sie aus diesem Grund sicher, dass Sie ein Backup erstellen oder einen Systemwiederherstellungspunkt erstellen, wenn etwas schief geht. Hier erfahren Sie, wie Sie Windows SmartScreen in acht einfachen Schritten deaktivieren können.

Schritt 1


Öffnen Sie die Windows-Registrierung, indem Sie die Windows-Taste + R drücken, um run zu öffnen und regedit einzugeben. Sie können auch mit der rechten Maustaste auf das Windows-Symbol klicken und Ausführen auswählen.

Schritt 2


Der Windows Registry Editor wird geöffnet. Fahren Sie fort, Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\System in den Pfad zu kopieren und einzufügen, wie durch das rote Kästchen in Ihrem Windows Registry Editor angezeigt. Drücken Sie Enter.



Schritt 3

<img src="/windows-sicherheitscenter-suche.png" alt="windows sicherheitscenter suchen">

Erstellen von dword value
DWORD (32-Bit) Wert erstellen
Klicken Sie mit der rechten Maustaste auf den weißen Bereich in der rechten Seitenleiste. Erstellen Sie dann einen neuen DWORD (32-Bit) Wert-Schlüssel.

Schritt 4

dword umbenennen
Umbenennen von DWORD
Fahren Sie fort, den DWORD-Schlüssel in EnableSmartScreen umzubenennen.

Schritt 5

Ändern des dword
Ändern des DWORTes
Doppelklicken Sie auf den neu erstellten Schlüssel EnableSmartScreen, um ihn zu bearbeiten. Geben Sie unter Wertdaten 0 zum Deaktivieren oder 1 zum Aktivieren ein.

Schritt 6

Erstellen des Zeichenkettenwertes
Erstellen des Zeichenkettenwertes
Klicken Sie mit der rechten Maustaste auf das gleiche rechte Seitenfenster, um einen neuen Zeichenkettenwert zu erstellen.

Schritt 7

<img src="/string_value_umbenennen.png" alt="windows sicherheitscenter suchen">

Umbenennen des Zeichenkettenwertes
Umbenennen des Zeichenkettenwertes
Benennen Sie den neuen String Value ShellSmartScreenLevel um.

Schritt 8

Setzen des Zeichenkettenwertes
Einstellen des Wertes für die Zeichenkette
Doppelklicken Sie auf ShellSmartScreenLevel, um es zu bearbeiten. Unter Wertdaten können Sie Block, Warnung oder Aus eingeben. Aus deaktiviert die Warnmeldung, wenn eine nicht erkannte Anwendung ausgeführt wird.

Deaktivieren über den Editor für lokale Gruppenrichtlinien
Für Benutzer von Windows 10 Pro und Enterprises können Sie den Windows Smartscreen über den Local Group Policy Editor deaktivieren.

Drücken Sie die Tasten Windows + R oder geben Sie RUN in die Suche ein, indem Sie auf die Schaltfläche Search Lupe im Aufgabenmenü klicken.
Sobald RUN geöffnet ist, geben Sie gpedit.msc ein und klicken Sie auf OK.
Ein Editor für lokale Gruppenrichtlinien wird dann geöffnet.
Navigieren Sie zu Computerkonfiguration > Administrative Vorlagen > Windows-Komponenten > Datei-Explorer.
Wählen Sie Configure Windows Defender SmartScreen und doppelklicken Sie darauf, um die Einstellungen zu öffnen.
Aktivieren Sie in den Richtlinieneinstellungen das Optionsfeld Deaktiviert und klicken Sie auf OK.
Wählen Sie unter den Optionen "Warnung und Vermeidung von Bypass".
Schließen Sie den Editor für lokale Gruppenrichtlinien und starten Sie Ihren Computer neu, damit Änderungen wirksam werden.

