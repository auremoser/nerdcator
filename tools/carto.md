# Carto
* [English Version](#english)
* [German Version](#german)
* [Greek Version](#greek)

## English

*CARTO* is an open, powerful, and intuitive platform for discovering and predicting the key insights underlying the location data in our world. While it is a commercial tool, there is also a free account option, which allows you to easily and beautifully display data on a map. For collecting the data one could utilize different ways, for demo purposes we stuck to *Google Forms* for now, but *Carto* does offer endpoints for easily dragging in data from other sources as well.

### Collecting & Visualizing Data
![google forms](../images/carto/form-bastian.png)

Both Bastian & Aurelia gave this option a a try. By setting up a simple *Google Form* people can either enter data through adding the latitude or longitude ([see Bastian's form](https://docs.google.com/forms/d/e/1FAIpQLSe0e_H-pTPVqVlQK-R-hvuMKn9zyPJ2OpqJ0efL1hPYDhx6BQ/viewform)) or by using the street-level geocoding function ([see Carto Docs](https://carto.com/docs/carto-engine/dataservices-api/geocoding-functions/#street-level-geocoder)).

![google spreadsheet](../images/carto/spreadsheet-bastian.png)

![carto-google-endpoint](../images/carto/carto-connect-bastian.png)

In either case, you will end up with a *Google Spreadsheet* that contains the data points entered through the form. These can then easily be linked to *Carto* using their *Google Drive*-endpoints.

![carto-map-bastian](../images/carto/carto-map-bastian.png)

This data can [then be shown on the *Carto*-map](https://gedankenstuecke.carto.com/viz/1312f3ba-8eba-11e6-b515-0ef7f98ade21/public_map). If you added categories to the *Google Form*, you can assign different symbols for the display on the map. In addition you can also select which data points should be in the tooltips displayed on the map. [Aurelia's map can be found here](https://auremoser.carto.com/builder/fe0d9b1c-9082-11e6-aeba-0e3ebc282e83/embed
).

Some instructions from the [etherpad](https://gedankenstuecke.piratenpad.de/nerdcator)


### Pros
* can easily display the data
* looks pretty beautiful out of the box
* One can in principle even implement a search function
* choosing the Google Drive option for adding a new dataset
* once the form results are sync'd, you could set up a trigger to automatically fill in the_geom field using the street-level geocoding function: <https://carto.com/docs/carto-engine/dataservices-api/geocoding-functions/#street-level-geocoder>
* use `UPDATE nerdcator_entry_form_responses SET the_geom = cdb_geocode_street_point(where_is_this_place_full_address_with_number_city_state_co)` to update dynamically
* styling is nice, and you can add the form responses to the tooltip, easy

### Cons
* It doesn't geocode correctly always, and geocoder won't let you manually edit geom values while syncing.
* automatic sync of a *Google Spreadsheet* to *Carto* is only possible in the paid version.
* data entry through google form is cumbersome

## German

*CARTO* ist eine offene, mächtige und intuitive Platform um Geodatenzu visualisieren etc. Neben einer bezahlten Version gibt es eine kostenlose Einsteiger-Variante, welche ausreicht um Daten einfach auf einer Karte anzuzeigen. Um unsere Geodaten zu sammeln haben wir uns für *Google Forms* entschieden, dank der vielfältigen Import-Möglichkeiten von *Carto* könnte eins diese aber auch auswechseln.

### Sammeln & Visualisieren unserer Daten  Data
![google forms](../images/carto/form-bastian.png)

Sowohl Bastian als auch Aurelia haben es ausprobiert. Mit einem einfachen *Google Form* kann eins Daten entweder per Längen- und Breitengrad hinzufügen ([siehe Bastians Formular](https://docs.google.com/forms/d/e/1FAIpQLSe0e_H-pTPVqVlQK-R-hvuMKn9zyPJ2OpqJ0efL1hPYDhx6BQ/viewform)) oder mit Hilfe der *street-level geocoding* Funktion ([siehe Carto Docs (english)](https://carto.com/docs/carto-engine/dataservices-api/geocoding-functions/#street-level-geocoder)).

![google spreadsheet](../images/carto/spreadsheet-bastian.png)

![carto-google-endpoint](../images/carto/carto-connect-bastian.png)

In beiden Fällen bekommt mensch ein *Google Spreadsheet* welches die Datenpunkte enthält. Dieses kann mensch einfach in Carto importieren, dank des *Google Drive*-Importers.

![carto-map-bastian](../images/carto/carto-map-bastian.png)

Die so importierten Daten [können dann auf der Carto-Karte angezeigt werden](https://gedankenstuecke.carto.com/viz/1312f3ba-8eba-11e6-b515-0ef7f98ade21/public_map). Wenn das *Google Spreadsheet* Kategorien enthalten hat kann mensch verschiedenen Kategorien auch verschiedene Icons zuordnen. Dazu kann eins auswählen welche Informationen auf in den Tooltips auf der Karte angezeigt werden sollen. [Aurelia's Karte kann mensch hier sehen](https://auremoser.carto.com/builder/fe0d9b1c-9082-11e6-aeba-0e3ebc282e83/embed
).

Ein paar mehr (englische) Anmerkungen gibt es im Etherpad [etherpad](https://gedankenstuecke.piratenpad.de/nerdcator).


### Vorteile
* Mensch kann die Daten einfach visualisieren
* Ist ohne viel Aufwand hübsch
* Mensch könnte relativ einfach eine Such-Funktion einfügen
* Von Google Drive kann mensch Daten einfach importieren
* Mensch könnte die Street-Level Geokodierung nutzen, siehe https://carto.com/docs/carto-engine/dataservices-api/geocoding-functions/#street-level-geocoder
* `UPDATE nerdcator_entry_form_responses SET the_geom = cdb_geocode_street_point(where_is_this_place_full_address_with_number_city_state_co)` für dynamische Updates
* Das Design ist hübsch und kan kann die Form-Felder einfach zu Tooltips umwandeln.

### Nachteile
* Die automatischen Geocodierungen sind nicht immer korrekt und mensch kann sie nicht per Hand korrigieren beim Import
* Der automatische Sync von *Google Spreadsheet* zu *Carto* ist nur in der Bezahl-Version möglich.
* Die Dateneingabe mit Google Forms ist nicht sehr bequem



## Hindi
*maybe to come*

## Greek

Το *CARTO* είναι μία ανοιχτή, δυνατή και ενστικτώδης πλατφόρμα για την ανακάλυψη και πρόβλεψη σημείων ενδιαφέροντος που βρίσκονται σε κάποια τοποθεσία δεδομένων στο κόσμο μας. Παρότι είναι ένα εμπορικό εργαλείο, υπάρχει και μία επιλογή δωρεάν λογαριασμού, η οποία επιτρέπει να απεικονίσετε δεδομένα σε ένα χάρτη εύκολα και όμορφα. Για τη συλλογή δεδομένων θα μπορούσαν να χρησιμοποιηθούν διαφορετικοί τρόποι, αλλά για τους σκοπούς αυτού του demo μείναμε στα *Google Forms* προς το παρόν, αν και το *CARTO* παρέχει τρόπους για να εισάγετε δεδομένα κι από άλλες πηγές.

### Συλλογή και απεικόνιση δεδομένων
![google forms](../images/carto/form-bastian.png)

Ο Bastian και η Aurelia δοκίμασαν αυτή την επιλογή. Εγκαθιστώντας μία απλή *Google Form* θα μπορούσατε να εισάγετε δεδομένα προσθέτοντας γεωγραφικό πλάτος και μήκος ([βλέπε τη φόρμα του Bastian](https://docs.google.com/forms/d/e/1FAIpQLSe0e_H-pTPVqVlQK-R-hvuMKn9zyPJ2OpqJ0efL1hPYDhx6BQ/viewform)) ή χρησιμοποιώντας τη geocoding λειτουργία στο επίπεδο δρόμου ([βλέπε Carto Docs](https://carto.com/docs/carto-engine/dataservices-api/geocoding-functions/#street-level-geocoder)).

![google spreadsheet](../images/carto/spreadsheet-bastian.png)

![carto-google-endpoint](../images/carto/carto-connect-bastian.png)

Εν πάσει περιπτώσει, θα καταλήξετε με ένα *Google Spreadsheet* που περιέχει τα δεδομένα που έχουν εισαχθεί από τη φόρμα. Αυτά μπορούν να συνδεθούν εύκολα με το *Carto* χρησιμοποιώντας τα *Google Drive*-endpoints τους.

![carto-map-bastian](../images/carto/carto-map-bastian.png)

Τα δεδομένα μπορούν [να απεικονιστούν στα *Carto*-map](https://gedankenstuecke.carto.com/viz/1312f3ba-8eba-11e6-b515-0ef7f98ade21/public_map). Αν προσθέσατε κατηγορίες στη *Google Form*, μπορείτε να αναθέσετε διαφορετικά σύμβολα για την απεικόνιση των δεδοένων στο χάρτη. Επίσης, μπορείτε να επιλέξετε ποια σημεία θα έπρεπε να να απεικονιστούν στις επεξηγήσεις του χάρτη.  [Μπορείτε να βρείτε το χάρτη της Aurelia εδώ](https://auremoser.carto.com/builder/fe0d9b1c-9082-11e6-aeba-0e3ebc282e83/embed
).

Μερικές οδηγίες από το [etherpad](https://gedankenstuecke.piratenpad.de/nerdcator)

### Υπέρ
* Μπορεί να απεικονίσει εύκολα δεδομένα
* Δείχνει αρκετά όμορφο αμέσως
* Νέα datasets μπορούν να προστεθούν μέσω της επιλογής *Google Drive*
* Μόλις τα αποτελέσματα των πεδίων συγχρονιστούν, θα μπορούσε να υλοποιηθεί ένα trigger για αυτόματη συμπλήρωση του πεδίου _geom χρησιμοποιώντας τη λειτουργία geocoding σε επίπεδο δρόμου: <https://carto.com/docs/carto-engine/dataservices-api/geocoding-functions/#street-level-geocoder>
* Δυναμική ενημέρωση χρησιμοποιώντας: `UPDATE nerdcator_entry_form_responses SET the_geom = cdb_geocode_street_point(where_is_this_place_full_address_with_number_city_state_co)`
* Ωραίο στυλ, και οι απαντήσεις στις φόρμες μπορούν να χρησιμοποιηθούν στις επεξηγήσεις, εύκολα

### Κατά
* Η γεωκωδικοποίηση δεν είναι πάντα σωστή, και δεν επιτρέπει να επεξεργαστούν χειροκίνητα οι γεωγραφικές τιμές ένω συγχρονίζεται
* Αυτόματος συγχρονισμός ενός *Google Spreadsheet* στο *Carto* είναι δυνατή μόνο στην εκδοχή επί πληρωμής
* Η εισαγωγή δεδομένων μέσω google form είναι δύσκολη

