# enigma2-python3
Python 3 Install Script openATV

Erst mal schauen was für ein Paketdienst läuft.

Gebt nachfolgendes ein:

    apt list
    
Ist die Ausgabe „command not found“ habt ihr ein altes Enigma 1.6 bis 2.0 drauf oder einen alten Paketmanager.

Gebt dann nachfolgendes ein:

     opkg list
     
jetzt müsste allerhand an Text ausgeben werden.

Wollt ihr eine Liste als Text Datei haben gebt bitte folgendes ein.

     cd /tmp
     opkg list>liste.txt

Jetzt habt ihr im Verzeichnis /tmp eine Textdatei mit dem Namen „liste.txt“ die ihr euch anschauen könnt.

Genauso geht das wenn ihr nachschauen wollt was auf eurem Receiver installiert ist.

     cd /tmp
     opkg list-installed>installiert.txt

Jetzt habt ihr im Verzeichnis /tmp eine Textdatei mit dem Namen „installiert.txt“ die ihr euch anschauen könnt.

Python 3 installieren:

Erst mal schauen was für ein Python 3 möglich ist.

     opkg list | grep python3
     
oder wieder als liste.

     cd /tmp
     opkg list | grep python3>py3liste.txt

py3-installer-xxx.sh  Python 3 openATV Installationsskript für opkg Installierung, 

bitte Ausfürbar machen und mit ./py3-installer.sh starten.

Wenn ihr den apt Paketmanager habt, müst ihr opkg in apt umbenennen.
