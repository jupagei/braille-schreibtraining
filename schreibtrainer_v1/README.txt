
Ansichtswechsel:
- Bei Lernmodul 2/3/4 wird jetzt das Hauptmenü ausgeblendet.
- Statt eines eingeblendeten Untermenüs erscheint eine eigene Auswahlansicht mit zwei Optionen.
- Der Zurück-Button führt wieder zur Hauptauswahl zurück.

Weitere Anpassung:
- In den Auswahlansichten für Lernmodul 2, 3 und 4 steht "Alle bisherigen Zeichen" jetzt immer links.

Überlebensmodus v14:
- Eigene dezente Hintergrundmusik im Überlebensmodus.
- Keine maximale Aufgabenanzahl mehr.
- Zufällige Zeichen aus allen Lernmodulen laufen unbegrenzt.
- Richtiges Feedback zeigt ausschließlich die aktuelle Streak.
- Ab 10: 🔥, ab 50: 🔥🔥, ab 100: 🔥🔥🔥.
- Bei einer falschen Antwort endet die aktuelle Streak und eine neue beginnt bei 0.

Navigation v18:
- "Startmenü"-Button unten links in Zwischenmenüs und Übungsansicht ergänzt.
- Der sichtbare Button "➡️ Nächstes Zeichen" wurde entfernt.
- Richtige Antworten wechseln weiterhin automatisch zur nächsten Aufgabe.
- Nach Abschluss einer normalen Runde bleibt "🔄 Noch eine Runde" verfügbar.

Musik v22:
- Die bisherige dezente Hintergrundmusik läuft jetzt in allen normalen Lernmodulen.
- Der Überlebensmodus hat eine neue, etwas energischere eigene Hintergrundmusik.
- Beim Wechsel zurück ins Startmenü wird die Musik beendet.

Layout v23:
- Feste übergroße Bühnenhöhe entfernt.
- Die gemeinsame Bühne passt ihre Höhe jetzt dynamisch an die aktive Ansicht an.
- Startmenü und Übungsansicht sind dadurch größenmäßig näher beieinander.
- Höhenwechsel bleiben weich animiert, damit keine harten Sprünge entstehen.

Anzeige v24:
- Das kleine schwarze Braille-Unicodezeichen unter der großen Braillezelle wurde entfernt.
- Stattdessen wird die Punktnotation angezeigt, z. B. P1, P12, P13456.
- Mehrzellige Eingaben werden z. B. als P4 · P345 dargestellt.

Ergänzung:
- GB in Lernmodul 1, Punkte 45, Audio: audio/m1_gb.mp3
- GW in Lernmodul 4, Punkte 46, Audio: audio/m4_gw.mp3

Musikschalter:
- In der Übungsansicht kann die Hintergrundmusik jederzeit deaktiviert und wieder aktiviert werden.
- Der Schalter betrifft nur die Hintergrundmusik; Zeichenansagen und Feedbacksounds bleiben aktiv.
- Die Einstellung gilt gleichermaßen für normale Zeichensätze und den Überlebensmodus.

Musik v42:
- Der Musikschalter befindet sich jetzt ausschließlich im Hauptmenü.
- Das Hauptmenü nutzt eine eigene Hintergrundmusik (audio/survival_background.wav).
- Beim Start eines Zeichensatzes wechselt die Musik automatisch zur jeweiligen Lern- bzw. Überlebensmodus-Musik.
- Beim Zurückkehren ins Hauptmenü startet wieder die Hauptmenü-Musik, sofern Musik aktiviert ist.
- Zeichenansagen und Feedbacksounds sind vom Musikschalter nicht betroffen.

Musik v43:
- Das Hauptmenü verwendet jetzt eine neu erzeugte, eigenständige Hintergrundmusik.
- Datei: audio/menu_background.wav
- survival_background.wav wird nicht mehr als Hauptmenü-Musik verwendet.

Tastenfeedback v45:
- Alle Tasten eines eingegebenen Braille-Chords bleiben nach dem Loslassen kurz gemeinsam lila sichtbar.
- Dadurch verschwinden bei leicht versetztem Loslassen keine gedrückten Tasten mehr aus der Anzeige.
- Bei einer falschen Eingabe werden zusätzlich falsch gedrückte Tasten kurz rot markiert.
- Nicht gedrückte, aber für die richtige Lösung fehlende Tasten werden nicht rot markiert.

Zuordnungskorrektur v46:
- äu: Audio m3_aeu_mit_ae.mp3, Braille P34.
- eu: Audio m3_eu_mit_e.mp3, Braille P126.
- Die Dateien wurden neu benannt, um Browser-Caching älterer Versionen auszuschließen.
- Die Zuordnung gilt damit identisch in Zeichensatz 3, 'Alle bisherigen Zeichen' und im Überlebensmodus.

Musikstatus-Fix v47:
- Wenn die Hintergrundmusik deaktiviert wurde, bleibt sie auch nach Rückkehr ins Hauptmenü und erneutem Start deaktiviert.
- Beim Wechsel zwischen Hauptmenü, Lernmodus und Überlebensmodus wird der aktuelle Musikstatus zentral synchronisiert.
- Alte Musikspuren werden vor jedem Wechsel vollständig gestoppt.
- Der Musikschalter zeigt jederzeit den tatsächlichen Zustand an.

Menümusik-Startfix v48:
- Die Hauptmenü-Musik wird beim Laden vorab vorbereitet.
- Sie startet bei der ersten echten Nutzerinteraktion im Hauptmenü (Maus, Touch oder Tastatur).
- Danach kann sie bei Rückkehr ins Hauptmenü wieder automatisch starten.
- Ein Aus-/Einschalten des Musikschalters ist dafür nicht mehr nötig.
- Browser-Autoplay-Regeln werden weiterhin berücksichtigt.

Tastenfeedback v49:
- Zusätzlich falsch gedrückte Tasten werden jetzt amberfarben statt rot markiert.
- Die Rückmeldung bleibt deutlich, wirkt aber weniger streng und passt besser zum warmen Fehlerfeedback.

Feedbacklogik v50:
- Normale Trainingsmodi: keine farbliche Markierung falsch gedrückter Tasten.
- Beim Klick auf „Lösung anzeigen“ werden die zur richtigen Lösung gehörenden Tasten amberfarben markiert.
- Überlebensmodus: zusätzlich falsch gedrückte Tasten werden weiterhin markiert, jetzt in gedämpftem Coral statt Amber.
- Lila bleibt die Farbe für aktuell gedrückte Tasten.

Persistente Lösungsanzeige v51:
- Nach Klick auf „Lösung anzeigen“ bleiben sowohl die Braille-Lösung als auch die amberfarben markierten richtigen Tasten sichtbar.
- Auch weitere falsche Eingaben blenden die Hilfe nicht aus.
- Erst nach einer richtigen Eingabe wird die Hilfe entfernt und mit der nächsten Aufgabe fortgefahren.

Feedbacklogik v52:
- Die farbliche Markierung falsch gedrückter Tasten wurde vollständig entfernt, auch im Überlebensmodus.
- Lila bleibt die Farbe für aktuell gedrückte Tasten.
- Amber wird ausschließlich als Hilfefarbe nach „Lösung anzeigen“ verwendet.

Layout-Anpassung v53:
- Die Lösungsanzeige erscheint jetzt direkt unter der Braillezelle / Punktanzeige.
- Die Lösung ist amberfarben gestaltet und damit klar als Hilfefarbe gekennzeichnet.
- Die Tastenhilfe bleibt wie bisher bestehen, wenn „Lösung anzeigen“ gewählt wurde.

Anpassungen v54:
- Das große Zeichen unter der Braillezelle zeigt jetzt die eingegebene Braille-Unicode-Schreibweise statt PXXX.
- Die Hilfsanzeige nach „Lösung anzeigen“ zeigt nun PXXX in Amber, ohne den Zusatz „Lösung“.
- Im Überlebensmodus werden bei falscher Eingabe kurz alle zur richtigen Lösung gehörenden Tasten amberfarben eingeblendet.
- Wenn die Lösung einmal angezeigt wurde, bleibt sie im normalen Trainingsmodus auch bei weiteren Fehlversuchen sichtbar.

Anpassungen v55:
- Normalmodus: Unter der Braillezelle wird nach „Lösung anzeigen“ jetzt das Braillezeichen angezeigt.
- Überlebensmodus: Das amberfarbene Hilfesignal unter der Braillezelle zeigt kurz das korrekte Braillezeichen.
- Im gelben Feedbackkasten des Überlebensmodus steht nun der Punktcode (PXXX) statt des Braillezeichens.
- Die Lösungszeile unter der Braillezelle reserviert dauerhaft Platz, wodurch Ein- und Ausblenden ruhiger wirken.

Anpassung v56:
- Im Überlebensmodus wird bei falscher Eingabe die lilafarbene Anzeige der eingegebenen Braillezeichen ausgeblendet.
- Sichtbar bleibt nur das korrekte Braillezeichen in Amber sowie der Punktcode im gelben Feedbackkasten.

Anpassungen v57:
- Die lilafarbene Zwischenanzeige wurde in allen Modi entfernt.
- An derselben Stelle erscheint nun nur noch bei „Lösung anzeigen“ bzw. im Überlebensmodus bei Fehlern das korrekte Braillezeichen in Amber.
- Die separate zusätzliche Lösungszeile wurde entfernt; es gibt jetzt nur noch eine einzige Anzeige an dieser Position.

Anpassungen v58:
- Die eingeblendeten Braillezeichen bei den Lösungen sind größer und zentrierter gesetzt.
- Der Anzeigebereich unter der Braillezelle hat jetzt eine feste Höhe, damit Einblendungen ruhiger wirken und weniger ruckeln.
- Die Punktcodes im gelben Feedbackkasten wurden auf die normale Feedbackgröße reduziert.

Anpassungen v59:
- Die Zentrierung des Feedbacks wurde durch ein grid-basiertes Layout präzisiert.
- Die eingeblendeten Braillezeichen sind größer und in einer festen, mittig ausgerichteten Zeile platziert.
- Zusätzliche Laufweite bei Punktcodes und Hilfs-Braillezeichen wurde entfernt, damit beide optisch mittiger wirken.

Anpassungen v60:
- Die eingeblendeten Braille-Lösungszeichen werden jetzt in einem eigenen, exakt mittig positionierten Span gerendert.
- Für Braillezeichen wird eine passende Symbolschrift bevorzugt; eine kleine optische Korrektur gleicht die asymmetrischen Zeichenränder aus.

Anpassung v61:
- Die eingeblendeten Braillezeichen wurden minimal nach links korrigiert, sodass ihr optisches Zentrum mit dem Zentrum der darüberliegenden Braillezelle übereinstimmt.

Anpassungen v62:
- Die eingeblendeten Braillezeichen wurden minimal nach links verschoben, damit ihr optisches Zentrum besser mit dem Zentrum der großen Braillezelle übereinstimmt.
- Die stilisierten Leerpunkte in der Braillezellen-Anzeige wurden entfernt; sichtbar sind nun nur noch die tatsächlich gesetzten Punkte.

Anpassungen v64:
- Fehler aus v63 behoben: Tastatureingabe funktioniert wieder.
- Normalmodus: Lösungstasten werden mit lila Umrandung markiert.
- Überlebensmodus: Lösungstasten bleiben weiterhin amberfarben markiert.

Anpassungen v65:
- Die stilisierten Leerpunkte in der oberen Braillezelle wurden wiederhergestellt.
- Die eingeblendeten Braillezeichen im Hilfebereich sind nun wieder lila statt amberfarben.
- Die Lösungstasten bleiben im normalen Modus lila umrandet und im Überlebensmodus amber markiert.

Anpassungen v66:
- Die eingeblendeten Braillezeichen wurden noch einmal minimal nach links verschoben, damit ihr Zentrum besser mit der oberen Braillezelle übereinstimmt.

Anpassungen v67:
- Die kleine Hilfsanzeige unter der großen Braillezelle zeigt jetzt den Punktcode statt nochmals Braillepunkte.
- Das gilt sowohl im normalen Modus nach „Lösung anzeigen“ als auch im Überlebensmodus nach einer falschen Eingabe.
- Im Überlebensmodus zeigt der gelbe Feedbackkasten wieder „Vorsicht! 😯“ an; der Punktcode erscheint separat unter der großen Braillezelle.

Anpassungen v68:
- Die hervorgehobenen Lösungstasten bei falscher Antwort im Überlebensmodus wurden von Amber auf einen hellen Rosaton umgestellt, passend zum Überlebensmodus-Kartenstil.

Anpassungen v69:
- In den normalen Modulen wurde die bisher lila Umrandung der Lösungstasten auf eine rosane Umrandung umgestellt.
- Die rosa Markierung im Überlebensmodus bleibt bestehen.

Anpassungen v71:
- Unter der großen Braillezelle wird jetzt standardmäßig der eingegebene Punktcode in Lila angezeigt.
- Nach „Lösung anzeigen“ wechselt die Anzeige auf den richtigen Punktcode in Rosa und bleibt dort bis zur richtigen Eingabe stehen.
- Im Überlebensmodus wird bei falscher Antwort ebenfalls der richtige Punktcode in Rosa eingeblendet, während der Feedbackkasten weiterhin „Vorsicht! 😯“ zeigt.
- Bei bereits richtiger Eingabe erfolgt kein zusätzlicher Wechsel; die aktuelle Anzeige bleibt bis zur nächsten Aufgabe bestehen.

Anpassungen v72:
- Die Feedbackkästen wurden entfernt; Rückmeldungen erscheinen jetzt nur noch als eingeblendeter Text.
- Positive Rückmeldungen werden grün angezeigt.
- Falsche Rückmeldungen werden rosa angezeigt, auch im Überlebensmodus.

Anpassungen v73:
- Die Feedbackkästen wurden wieder ergänzt, jetzt aber deutlich kompakter und nur so groß wie für den jeweiligen Feedbacktext nötig.
- Positive Rückmeldungen erscheinen in einem kleinen grünen Kasten, falsche Rückmeldungen in einem kleinen rosa Kasten.
- Der eingegebene Punktcode bleibt bei richtiger Eingabe bis zur nächsten Aufgabe sichtbar; dadurch funktioniert die PXXX-Anzeige der Tasteneingabe nun auch beim Bestätigen korrekt.

Anpassungen v74:
- Fehler behoben: Der eingegebene Punktcode wird nach einer Tasteneingabe nicht mehr sofort wieder gelöscht.
- Der tatsächlich eingegebene Punktcode erscheint nun zuverlässig in Lila.
- Bei einer falschen Eingabe im normalen Modus bleibt der eingegebene Punktcode sichtbar, obwohl die Braillezellen für den nächsten Versuch zurückgesetzt werden.
- Die Lösungsanzeige in Rosa bleibt unverändert.

Anpassungen v75:
- Die Anzeige des eingegebenen Punktcodes bleibt jetzt auch bei richtigen Eingaben sichtbar, bis die nächste Aufgabe geladen wird.
- Das ungewollte Leeren der PXXX-Anzeige nach jeder Eingabe wurde entfernt.
- Die Eingabeanzeige wurde für flüssigeres Verhalten optimiert: weniger DOM-Neuaufbau, gecachte Tastenelemente und leicht schnellere Höhenanpassung.

Anpassungen v76:
- Bei mehrzelligen Zeichen wird die Lösungshilfe jetzt schrittweise dargestellt: zunächst nur die Tastenkombination der ersten Zelle, nach korrekter Eingabe die der nächsten Zelle.
- Der rosa richtige Punktcode wechselt dabei parallel zur jeweils aktuellen Lösungszelle.
- Im Überlebensmodus werden bei falscher Antwort die korrekten Tastenkombinationen und Punktcodes bei mehrzelligen Zeichen nacheinander eingeblendet statt gleichzeitig.
- Einzellige Zeichen verhalten sich unverändert.

Anpassungen v77:
- Die schrittweise Lösungseinblendung im Überlebensmodus wurde repariert.
- Bei mehrzelligen Zeichen wird Zelle 1 jetzt sofort angezeigt; danach folgen die weiteren Zellen nacheinander.
- Pro Schritt wechseln sowohl die rosa markierten Tasten als auch der rosa Punktcode zur jeweils nächsten Braillezelle.

Anpassungen v78:
- Die Überlebensmodus-Kachel im Hauptmenü wurde von Rosa auf Amber umgestellt (inklusive Hover- und Auswahlzustand).

Anpassungen v79:
- Der Überlebensmodus hat nun auch im Übungsbereich ein dezentes Amber-Farbschema (Progress, Writer-Rahmen, aktive Punkte, Tasten, falsches Feedback, Lösungshilfen und Vorlesen-Button).
- Die Streak-Anzeige wird ab 10 / 50 / 100 sichtbar stärker akzentuiert, ohne das Grundlayout zu verändern.

Anpassungen v80:
- Im Überlebensmodus bleibt bei einer falschen Eingabe nun zuerst für ca. 460 ms der tatsächlich eingegebene Punktcode sichtbar.
- Erst anschließend wechselt die Anzeige zur korrekten Lösung; bei mehrzelligen Zeichen weiterhin schrittweise von Zelle 1 zu Zelle 2.

Anpassungen v81:
- Die Lösungshilfe zeigt nun das korrekte Braillezeichen statt des korrekten Punktcodes; die eigene Eingabe bleibt weiterhin als lila Punktcode sichtbar.
- Im Überlebensmodus wurden Überschrift/Untertitel sowie die Tastendarstellung zusätzlich farblich an das Amber-Schema angepasst.

Anpassungen v82:
- Im Überlebensmodus wird bei falscher Antwort jetzt direkt nur noch die korrekte Lösung schrittweise angezeigt; der zuvor eingeblendete Punktcode der eigenen Eingabe entfällt dort.
- Der Startmenü-/Homebutton passt im Überlebensmodus nun ebenfalls zum Amber-Farbschema.

Anpassungen v83:
- Die eingeblendeten Lösungszeichen wurden wieder deutlich vergrößert.
- Die Braillezeichen sind nun wieder optisch mittiger ausgerichtet, damit ihr Zentrum besser mit der oberen Braillezelle übereinstimmt.

Anpassungen v84:
- Die schrittweisen Einblendungen bei doppelten Zeichen wurden verlangsamt, damit Zelle 1 und Zelle 2 leichter nacheinander verfolgt werden können.

Anpassungen v85:
- Im Überlebensmodus wird bei 0 nun statt „Überlebensmodus“ die Überschrift „Starte deine Streak!“ angezeigt.
- Die eingeblendeten Lösungszeichen wurden optisch weiter nach links ausgerichtet, damit sie mittiger unter der oberen Braillezelle sitzen.

Anpassungen v86:
- Die eingeblendeten Lösungszeichen wurden wieder auf die frühere, stimmigere optische Zentrierung zurückgesetzt.

Anpassungen v88:
- Die eingeblendeten Lösungszeichen werden nun als echte runde Punkte statt als Unicode-Braillezeichen dargestellt; dadurch wirken sie nicht mehr oval.
- In der Lösungshilfe werden keine leeren Punkte mehr angezeigt, sondern nur noch die tatsächlich gesetzten Punkte des korrekten Zeichens.

Anpassungen v89:
- Die eingeblendeten Lösungszeichen wurden noch einen kleinen Tick nach rechts verschoben, damit die optische Achse besser mit der oberen Braillezelle übereinstimmt.

Anpassungen v90:
- Die Überschrift bei einer 0er-Streak lautet nun „Beginne deine Streak!“.
- Der Feedback-Kasten für richtige Antworten ist im Überlebensmodus jetzt ebenfalls gelb/amberfarben.
- Die eingeblendeten Lösungszeichen wurden noch einen minimalen Tick nach rechts verschoben.

Anpassungen v91 – Performance:
- Die Braillezellen werden beim Tippen nicht mehr komplett neu aufgebaut, sondern im bestehenden DOM aktualisiert.
- Häufig verwendete Tastenelemente werden wiederverwendet statt wiederholt gesucht.
- Der ResizeObserver läuft im Übungsmodus nicht mehr permanent mit.
- Höhenanpassungen im Übungsmodus wurden gedrosselt und die Höhenanimation dort deaktiviert.
- Optik und Bedienlogik bleiben unverändert.

Anpassungen v92:
- Die Überschrift bei 0er-Streak lautet nun „Beginne deine Streak!“.
- Im Überlebensmodus erscheinen nun auch die positiven Streak-Einblendungen im gelben Feedback-Kasten wie „Vorsicht!“.
- Die eingeblendeten Lösungszeichen wurden noch minimal weiter nach rechts verschoben.

Anpassungen v93:
- Die eingeblendeten Lösungszeichen wurden nochmals minimal nach links verschoben (ca. 2 px), damit die Achse besser mit der oberen Braillezelle übereinstimmt.

Anpassungen v94:
- Die eingeblendeten Lösungszeichen wurden noch einen kleinen Tick nach rechts verschoben.
