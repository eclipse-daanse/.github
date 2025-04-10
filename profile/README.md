# 🌐 Eclipse Data Analysis Services (Daanse)

**Eclipse Daanse** is an open source software designed to analyze large amounts of data and extract valuable insights from it.

With a steady rise of digital data production in business, science and technology, the importance of data analysis has grown tremendously.

---

## 🛠️ Overview

Data Analysis Services offers a wide range of tools, technologies and expertise to interpret data in meaningful ways and help decision makers formulate strategies and identify patterns and trends.

---

## 🔍 Key Features

### 🧹 Data Cleansing and Integration
One of the crucial steps in data analysis is the preparation of the data. Often data are flawed or incomplete.  
Data Analysis Services helps to clean, transform and bring data into a unified form to enable sound analysis.

### 📊 Data Visualisation
Data can be complex and numbers alone are sometimes not enough to convey information.  
Data Analysis Services uses visualisation tools to present data in the form of charts, graphs and interactive dashboards.  
This simplifies the communication of results and insights.

### 📈 Statistical Analysis
Data Analysis Services uses statistical methods and models to analyse data and identify patterns, correlations or significance.  
This includes descriptives, inferential statistics, regression analysis, time series analysis and more.

### 💼 Business Intelligence
Data Analysis Services helps management to extract business-critical insights that help improve business processes, optimise resources and identify new business opportunities.

### 💾 Big Data Analysis
In a world characterised by huge amounts of data, Big Data analysis is an integral part of Data Analysis Services.  
Processing and analysing large and complex data sets require specialised tools and technologies.

---

## 🧩 Technologies

### 📡 XMLA (XML for Analysis)

XMLA provides a detailed specification for accessing analytical data sources.  
This specification describes the structure of XMLA messages and the supported operations for accessing OLAP data sources.  
The Test and Compatibility Kit (TCK) can be used to check compliance of different implementations with the XMLA specification and to ensure interoperability between systems.  
Eclipse Daanse offers a Java API via Jakarta XML Bind and flexible customisable SOAP messages.

### 🧮 MDX (Multidimensional Expressions)

MDX is a query language for multidimensional data sources and is closely related to XMLA.  
The scope and delimitation of MDX are as follows:  
Strings can be converted into an implementation or API model using parsers.

---

## 📊 OLAP (Online Analytical Processing)

OLAP is a powerful technology widely used in data analysis and reporting.  
It is based on several important components:

- **DataCube Provider**: Enables the creation and provision of multidimensional data cubes that offer efficient and flexible data organisation for complex analyses.
- **Access and Security Model**: Regulates access rights to data sources and ensures that only authorised users can access the information they need, while sensitive data remains protected.
- **Calculation Model**: Enables complex calculations and aggregations to be performed on the multidimensional data.
- **Dynamic Function Model**: Allows dynamic functions to be used to respond to changes in data sources or query results.

> Parts of this implementation are a fork of the Pentaho Mondrian Project.

---

## 🗄️ Databases

Different databases can be integrated via **JDBC (Java Database Connectivity)**, which allows developers to interact with different databases by providing a standardised method for connecting and querying.

The **JDBC Database Dialect Abstraction Layer** makes it possible to work with different databases without having to worry about the specific syntax differences.

OLAP data can thus also be accessed by means of OLAP **database-schema mapping**.

---

## 🧑‍💻 Clients

Eclipse Daanse enables access to analytical data sources from various client applications.

In addition to the possibility of integrating your own applications using the client libraries (in several languages like **Java** and **TypeScript**), Eclipse Daanse includes:

- Its own **web client** for tables, charts and maps as well as dashboards
- The ability to connect further reporting tools via **adapters and templates**

---


- **Pixelgenaue Platzierung**: Jedes Widget kann absolut positioniert werden. Komplexe Layouts wie Infografiken oder mehrseitige Reports möglich
- **Responsives Layout**: Widget-Größen sind fix, aber die Positionierung passt sich an das jeweilige Endgerät an.

---

## 🧩 Verfügbare Widgets
### Basis-Widgets
- Rahmen, Abrundungen, Schatten sowie Transparenzen von Hintergrund und Schrift können individuell eingestellt werden. Farben und Schattenverläufe lassen sich zudem dynamisch über Variablen steuern – etwa abhängig von der Tageszeit. So kann beispielsweise die Ausrichtung und Länge eines Schattens oder die Helligkeit eines Widgets automatisch dem Sonnenstand angepasst werden.
- *Farben, Schatten und Transparenz dynamisch nach Uhrzeit und Variablen steuerbar.*

### Chart-Widgets
- Balkendiagramme 
- Liniendiagramme 
- Kreisdiagramme 

### Datentabellen
- Sortierung und Filterung pro Spalte
- Paginierung
- Spalten- und Zeilenformatierung
- Hervorhebung (Highlighting)
- Exportfunktionen (z. B. CSV)

### PivotTable (Excel-ähnlich)
- Auswahl eines OLAP-Cubes
- Frei konfigurierbare Dimensionen (Spalten, Zeilen, Filter)
- Measures (Kennzahlen) dynamisch einsetzbar
- Export der erzeugten Aggregationen
- Ideal für interaktive BI-Analysen.

### Icons
- Auswahl aus vordefinierten Symbolkatalogen
- Anpassung von Vorder- und Hintergrundfarben
- Nutzen von Icons zur semantischen Codierung von Zuständen.

### Image
- Darstellung von Bildern
- Anwendung von Bildfiltern wie Kontrast, Helligkeit, Unschärfe etc.
- Skalierung und Rahmung frei wählbar.

### Progress Bars & Gauges
- Visualisierung einfacher Messwerte
- Darstellung als Tacho, Fortschrittsbalken oder Zahl.
- Ideal für KPIs wie Geschwindigkeit, Temperatur, Auslastung.

### SVG
- Einbettung und Darstellung von SVG-Grafiken
- Farbmanipulation über Variablen
- Perfekt für stilisierte Icons und Vektorformen.

### Repeatable SVG
- Wiederholte Darstellung von SVGs anhand numerischer Werte
- Beispiel: 10 Personen als Symbol für einen Zählerstand
- Beliebige SVGs können verwendet werden, nicht nur Icons.
- einfache Darstellung von Mengeverhältnissen oder Skalen (Bewertung 3 von 5 Sternen)

### RichText
- Formatierter Text mit Einbettung von Variablen
- Freie Platzierung im Dashboard
- Einsatz für Überschriften, erklärende Texte oder interaktive Labels.

### Text
- Schlichter Text ohne Formatierung
- Integration von Variablen (z. B. dynamische Messwerte)
- Nützlich für einfache Beschriftungen

### Video
- Darstellung von Videos mit oder ohne Steuerungsbuttons
- Einbettung von Livestreams möglich

### Karten (Map)
- Darstellung georeferenzierter Daten
- Integration von:
  - OGC Maps (gerenderte Kartenbilder)
  - OGC Features (Geo-Objekte mit Attributen)
  - SensorThings-Standorten
  - CSV- und CML-Datenquellen
  - XMLA
- Individuelles Styling für alle Layer (Färbung, Transpartenz, Icons, Linien, Flächen, Sensorwerte)
- alle Layer gemeinsam darstellbar

### SampleWidget
- Platzhalter für zukünftige experimentelle Widgets
- zeigt nativ die Rohdaten der Connection an

### Example Infografics
![Bildschirmfoto vom 2025-04-09 23-31-41](https://github.com/user-attachments/assets/5240f9ee-306a-413d-8b8d-5072377eb626)


---

## 🔌 Datenverbindungen (Connections)

### OGC Maps
- Einbindung gerenderter Karten (z. B. WMS-Dienste)
- Anzeige in Kartenwidgets

### OGC Features
- Anzeige von Geo-Objekten wie Haltestellen, Gullideckeln, Bäumen etc.
- JSON-basiert
- Mit Geometrie, Name und Stammdaten

### SensorThings API
- Historische Zeitreihen (z. B. Temperaturverlauf)
- Sensorstammdaten (Typ, Standort, Einheit)
- Live-Daten über REST oder MQTT/Websocket
- Perfekt für Smart-City-Anwendungen.

### XMLA für Datacubes
- Zugriff auf Datenwürfel über XMLA-Schnittstelle
- Unterstützt Microsoft Analysis Services, Daanse OLAP Server u. a.
- Kompatibel mit PowerBI und Excel Pivot.

### SQL über XMLA
- Ausführung von SQL-Statements über XMLA-Protokoll
- Rollenbasiertes Rechtemanagement
- Sicherheitsfunktionen gegen Missbrauch

### REST CSV
- REST-Schnittstelle zum Import von CSV-Dateien
- Auswahl von Delimiter
- Teilweises Einlesen großer Dateien möglich (Bereiche)

### REST JSON & XML
- Einfache REST-Anbindung für gängige APIs
- Unterstützt JSON und XML
- Kompatibel mit Open Government APIs, z. B. Mängelmelder, Verkehrsdaten.

### Semantic Web / SPARQL / RDF
- Zugriff auf Wikidata, DCAT, GovData, Open Energy Platform etc.
- Nutzung semantischer Abfragen über SPARQL
- Verknüpfung mit Linked Open Data.

### MQTT (plain)
- Direkte Verbindung zu MQTT-Brokern
- Empfängt Nachrichten bei Wertänderung
- Unterstützt Last-Will-Nachrichten

### WebSocket (plain)
- Direkter Empfang von Nachrichten via WebSocket-Protokoll
- Verbindung zu Webservern möglich, z. B. bei Custom Events.

### RSS
- Einbindung strukturierter RSS-Feeds
- Darstellung von Datum, Kurztext, Langtext, Link
- Ideal für Veranstaltungskalender, Fahrplanänderungen etc.

### GraphQL
- Moderne, webbasierte Abfragesprache
- Selektives Abfragen und Filtern von Feldern
- Subscriptions (Live-Daten)

---

## 🔁 Variablen

- **Konstanten** (z. B. ID eines Sensors)
- **Berechnete Variablen** (Formeln auf andere Variablen)
- **Zeitbasierte Variablen** (z. B. Sonnenstand, Uhrzeit)
- **Ergebnisse aus Abfragen** (z. B. aktuelle Temperatur)

Alle Eigenschaften von Widgets und Dashboards sind variablenfähig.

Beispiel: Eine Schaltfläche wechselt zwischen verschiedenen Objekten, indem eine Variable aktualisiert wird. Alle Datenquellen passen sich automatisch an.

---

## ✨ Besonderheiten

### 💻 Client-Only – Keine Serverinstallation notwendig

Die Software läuft vollständig im Webbrowser – ganz ohne zusätzliche Serverkomponenten oder Backend.  
Es ist lediglich ein einfacher Webserver nötig, der die Anwendung ausliefert. Die gesamte Logik, Darstellung und Datenanbindung erfolgt direkt im Client.

### 🖥️ Auch als Desktop-App nutzbar

Da keine serverseitige Infrastruktur erforderlich ist, kann Daanse nicht nur als Webanwendung im Browser genutzt werden, sondern auch als:

- **Progressive Web App (PWA)**
- **Desktop-Client** für macOS, Windows und Linux (z. B. über DEB und RPM-Pakete)

Bereits heute stehen erste Paketformate zur Verfügung.  
Weitere Varianten wie **Flatpak** und **AppImage** sind bereits in Planung.

### 🛡️ Datenschutz und Rechte – ein entscheidender Vorteil der Client-basierten Lösung

Bei Eclipse Daanse erfolgt die gesamte Datenverarbeitung direkt im Browser – ohne zwischengeschalteten Server. Die Daten werden über offene Schnittstellen geladen und unmittelbar auf dem Endgerät des Nutzers visualisiert.  

Gerade im Kontext von **Open-Data- oder Urban-Data-Plattformen**, bei denen Daten über klar definierte öffentliche APIs bereitgestellt werden, ist das ein großer Vorteil:  
Es entfällt die Notwendigkeit, Daten ein zweites Mal zu speichern oder durch einen Server zu schleusen – und damit auch das Risiko doppelter Rechtestrukturen.

Im Gegensatz dazu benötigen serverbasierte Systeme wie **Grafana** oder **Apache Superset** häufig einen zentralen Nutzerzugang mit weitreichenden Rechten, um auf die zugrundeliegenden Schnittstellen zugreifen zu können.  
Dieser technische „Superuser" sieht oft mehr als vorgesehen – insbesondere wenn daraufhin ein separates Rechtemanagement in der Dashboard-Anwendung aufgebaut wird, das nicht mit dem originalen API-Rechtesystem übereinstimmt.  

Das birgt ein erhebliches Sicherheitsrisiko: Ein Nutzer der Dashboard-Anwendung kann ungewollt Zugriff auf Daten erhalten, die er über die ursprüngliche API nie sehen dürfte.

**Daanse vermeidet dieses Problem vollständig** – durch direkten, autorisierten Zugriff aus dem Browser und durch Verzicht auf eigene Serverinfrastruktur.


### 🌍 Direkter Zugriff auf Open Data aus DCAT-Katalogen

In Open-Data-Plattformen wie [data.europa.eu](https://data.europa.eu) oder [GovData.de](https://www.govdata.de) werden alle Datensätze und Dienste standardisiert im **DCAT-Schema** beschrieben.  

Der Daanse Board-Client kann diese öffentlichen **DCAT-Registries direkt abfragen** – etwa nach Begriffen wie *„Feuerwehreinsätze"*.  
Gefundene Datensätze oder Dienste können unmittelbar eingebunden und visualisiert werden – ganz ohne aufwendige Schnittstellenkonfiguration.

Beim Erstellen eines Dashboards wird für jede ausgewählte Datenquelle automatisch eine Liste passender Widgets vorgeschlagen.  
Diese muss man nur noch auswählen – und erhält sofort eine fertige Visualisierung.

➡️ **Schneller, intuitiver und direkter Zugriff auf die gesamte Welt offener Daten.**

### 🔗 Zusammenführung mehrerer Datenquellen – im Dashboard und im Widget

#### 📊 Integration verschiedener Datenquellen in einem Dashboard

In einem einzelnen Dashboard lassen sich beliebig viele Datenverbindungen kombinieren – auch aus unterschiedlichen Typen und Städten. So können beispielsweise folgende Informationen gemeinsam dargestellt werden:

- **Geodaten** über OGC Maps und OGC Features (z. B. Stadtpläne, Haltestellen)
- **Echtzeit-Sensorik** wie das Öffnen und Schließen von Straßenbahntüren über SensorThings, WebSocket oder MQTT
- **Stammdaten** zu Haltestellen, Linien und Fahrzeugen über REST, GraphQL, SPARQL oder SQL
- **Statistiken zur Pünktlichkeit und Verspätung** über Datacubes (XMLA/BI) oder SQL
- **Historische Bewegungsdaten** von Fahrzeugen über SensorThings (zeitbasierte Abfragen)

Diese Kombination erlaubt ein ganzheitliches Verständnis urbaner Prozesse – live, historisch und analytisch zugleich.


#### 🧩 Kombination mehrerer Datenquellen in einem einzelnen Widget

Auch **innerhalb eines einzelnen Widgets** können mehrere Datenquellen aus unterschiedlichen Städten oder Systemen vereint werden. Beispiele:

- Eine **interaktive Karte**, die:
  - Geodaten vom Land (OGC Maps),
  - Echtzeitdaten einer Stadt (SensorThings) und
  - Statistische Daten vom Bundesamt (XMLA)
  gleichzeitig visualisiert.

- Eine **Tabelle**, die:
  - CSV-Daten über REST,
  - JSON-Daten über APIs,
  - SQL-Abfragen und
  - Datenwürfel-Ergebnisse  
  von verschiedenen Anbietern (z. B. mehreren Städten) nebeneinander darstellt.

Diese Funktion macht Daanse besonders stark in der **interkommunalen Zusammenarbeit** und bei der **Zusammenführung heterogener Datenwelten** auf einem Blick.

### Git-Integration
- Dashboards versionierbar und nachvollziehbar
- Unterschiedliche Varianten möglich (z. B. Fraktionen im Stadtrat)
- Änderungen sind dokumentiert und auditierbar


Alle Daten können transparent angezeigt werden, während Dashboards zum selben Thema und mit denselben Datenquellen individuell gestaltet werden können.
So kann beispielsweise jede Fraktion eines Stadtrats ihr eigenes Dashboard erstellen und dabei eine eigene inhaltliche Perspektive („Framing“) wählen – ohne dass sich die zugrundeliegenden Daten unterscheiden. Für die Nutzer bleibt stets nachvollziehbar, was die originalen Daten sind und worin sich die verschiedenen Darstellungen der Fraktionen unterscheiden.

Änderungen an Dashboards sind stets nachvollziehbar und auditierbar: Es lässt sich jederzeit nachvollziehen, wer wann was geändert hat. Zudem können Änderungen begründet und dokumentiert werden.
