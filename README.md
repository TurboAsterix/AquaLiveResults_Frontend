# AquaLiveResults_Frontend
AquaLiveResults: Live race results from Aquarius, frontend component

# Demo and Documentation
https://www.aqualiveresults.de/

# Was ist AquaLiveReuslts?
AquaLiveResults ermöglicht die (nahezu) Echtzeit-Anzeige von Regatta-Ergebnissen aus der im Rudersport weit verbreiteten Software Aquarius. 
Die Ergebnisse werden auf einer Webseite dargestellt, sodass Athleten, Publikum und Veranstalter sie direkt nach dem Zieleinlauf abrufen können ohne auf den Aushang der Ergebnisse zu warten.

# Frontend
Bei diesem Repository handelt es sich um die Frontend-Komponente, die auf dem Webserver deployed wird. 
Eine Webanwendung, die speziell für die Darstellung großer, responsiver und dynamisch geladener Tabellen optimiert ist und auf Smartphones, Tablets und Desktops funktioniert. 
Die Tabellenzeilen können expandiert werden um Titel, Lauf, Abteilung, Bahn und Namen der Mannschaft anzuzeigen.

# Backend
Work in progress 
  
# Daten
Die Backend-Komponente extrahiert die Rennergebnisse und aktualisiert (im Standard alle 3 Minuten) die Datei ./public/data/aquarius_db_output.json per SFTP.

# Webspace Voraussetzungen 
Fast keine. Statisches Datei-Hosting mit SFTP Zugang ist ausreichend. 
Die Tabelle wird vom Browser über eine Javascript Library gerendert (siehe unten Tabulator). 
Kein PHP, keine Datenbank etc.

# Aufruf
./public/tabulator_index.html ist die zentrale HTML Datei um die Tabelle anzuzeigen. Auf diese Datei sollte auf einer eigenen Landingpage verlinkt werden.

# Tabulator
Die AquaLiveResults Frontend Komponente nutzt zum Rendern der Tabelle der Rennergebnisse die JavaScript Library Tabulator in Version 6.4, die unter MIT License verfügbar ist.
https://www.tabulator.info 
https://www.tabulator.info/docs/6.4/license
https://github.com/olifolkerd/tabulator
