Things to do:
=============
* LDAP Login
* Lieferanten hinzufügen
    * Logindaten
    * Öffnungszeiten
    * Unsere Kontaktdaten (z.B. Frank Nord)
* Bestellung erstellen (Essen bestellen)
    * Datum/Uhrzeit angeben wann bestellt wird
        * editierbar machen
    * Bezahlmöglichkeiten bei dieser Bestellung fuer Member
        * Free / Bar / Paypal / BTC / Dogecoin
    * Mindestbestellwert
    * Maximal Bestelleranzahl?
    * Bestellung als abgeschickt markieren
    * Angegebene Lieferzeit des Lieferanten notieren
    * Bestellung abbrechen aus gründen
    * Trinkgeld fuer Lieferanten
* Bestellung annehmen
    * Liste der bestellten Dinge zum abbgleich
    * Warenwert + Trinkgeld
    * Mobile friendly
* Mit bestellen eines Members beim "Essen bestellen"
    * items einzeln hinzufügbar
    * Gesamtsumme je Member
    * Trinkgeld
* Notifkationen
    * An Ersteller der Essensbestellung das die Essensbestellungszeit erreicht ist
    * An Bar das eine Essensbestellung ausgeführt wird
    * An Besteller und alle mitbestellenden das Lieferung angekommen ist
    * c_out ansage in der Nerd
    * eigene Infobox like Barindikator
    * Bestellung wurde rausgeschickt, evtl mit angegebener Lieferzeit des Lieferanten
    * Bestellugn wurde abgebrochen, mit grund
* Tracking
    * Trackingmöglichkeit fuer Besteller wer schon bezahlt hat
        * auch Teilweise Zahlungen möglich machen
        * Erinnerungsmails an Besteller und Bestellenden nach 24 Stunden wenn nicht als Bezahlt markiert wurde
    * Bestellung als angekommen markieren / Lieferzeit
        * Uhrzeit editier machen falls man vergessen hat auf angekommen zu klicken
    * Gabs was gratis dazu?
    * Hats geschmekt
    * Hat der Lieferant uns gefunden?
    * Lieferung war vollständig
* Hübsche Graphen / Stats
    * Bestellzeit je Lieferant
        * aufschlüsselung nach Tagen / Uhrzeit
    * Anzahl der Bestellungen
        * je Lieferant
        * je Wochentag
        * je Woche
        * je Monat
    * Geld ausgegeben (heute, diese woche, dieser monat, je wochentag)
        * alle Lieferanten
        * je Lieferant
    * Wahrscheinlichkeits graph einer Bestellung nach uhrzeit
* System Integration
    * c-beam app notifikation wenn gewollt
    * c_out ansagen
    * REST API
    * c-beam #pizza suport 

Benutzergruppen
===============

* Der Besteller
* Die Mitbesteller
* Die Barcrew (wäre nett)

Datenstrukturen
===============

Lieferanten
    Name
    Addresse (Koordinaten)
    Telefonnummer
    Unser Kontaktdaten
    Unsere Accountdaten

Lieferanten Bestellung
    Lieferant
    Ersteller (member)
    Creation Date
    Order Date (orders can be added until this date)
    State

Member Bestellung
    Lieferanten Bestellung
    Member
    Items[
        Name
        evtl. Nummer
        Preis
        Anzahl
    ]

