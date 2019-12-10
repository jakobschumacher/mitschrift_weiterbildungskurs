---
layout: post
title:  "Räumliche Analyse in der GBE"
date:   2019-12-09 08:00:00 +0100
categories: Modul-2
permalink: gesundheitsgeographie/
autor: 210
---

# Was ist gesundheitsgeographie
_almost everything that happens, happens somewhere (Longley et al. 2005)_
_Everything is related to everything, but near things are more related than distant things._

* [The association between neighborhood economic hardship, the retail food environment, fast food intake, and obesity: findings from the Survey of the Health of Wisconsin (M. Laxy et al, 2015)](https://bmcpublichealth.biomedcentral.com/articles/10.1186/s12889-015-1576-x)
* [Differences in Male life Expectancy in London](https://tubecreature.com/#/livesontheline/current/same/U/*/FFTFTF/13/-0.1000/51.5200/)
* [Regionaler Deprivationsindex  German Index of multiple Deprivation (C. Hofmeister et al)](https://www.researchgate.net/publication/272749333_Regional_Deprivation_in_Germany_Nation-wide_Analysis_of_its_Association_with_Mortality_Using_the_German_Index_of_Multiple_Deprivation_GIMD) 
* Access to physicians walking distance (J. Schweikert Beuth Hochschule für Technik 2012)

# Was sind Geodaten
* Geodaten sind digitale Daten mit Raumbezug (Punkt, Linie, Fläche)
* Geodaten liegen als Schichten (Layer) vor
* Geodaten können mit Sachdaten (Attributen) verknüpft werden
* Geodaten bestehen aus Vektor- und Rasterdaten
  - Vektordaten sind viel einfacher
  - Rasterdaten sind für manche Fragestellungen sinnvoller

# Was bringen Geodaten
* Geodaten können Informationen über umweltbezogene Risiko- und Schutzfaktoren liefern
* Zusätzliche objektive Informationsinhalte aus dem geographischen Wohnumfeld
* Geodaten können neben der Auswertungsebene auch auf der Durchführungs- und Visualisierungsebene genutzt werden. 

# Welche Geodaten gibt es
* Amtliche Geodaten 
  - [Digitales Landschaftsmodell](https://gdz.bkg.bund.de/)
  - [Geoportal Berlin](https://www.stadtentwicklung.berlin.de/geoinformation/) 
* Wissenschschaftliche Geodaten (z.B. Satellitendaten)
* Kommerzielle Geodaten (z.B. von GfK)
* Freiwillig gesammelte Geodaten (z.B. aus OpenStreetMap)
* Weitere Datenquellen
  - [Landatlas](https://www.landatlas.de/)
  - Gemeindeverzeichnis 
  - [Deprivationsindex vom RKI](https://data.gesis.org/sharing/#!Detail/10.7802/1460) 

# Was sind Geoinformationssysteme
* Rechnergestützte Managementsysteme zur Verarbeitung von Daten mit Raumbezug
* Funktionen von GIS
  - Erfassen
  - Verwalten
  - Modifizieren
  - Analysieren
  - Visualisieren
  - Verbreiten
* Analysetechniken
  - Datenbankabfrage
  - Geometrische Berechnung
  - Verschneiden, Ausschneiden, Verbinden von Geometriedaten
  - Pufferbildung
  - Dichteschätzungen
  - Interpolation
  - Glättungen
  - Analyse raumbezogener Verteilung
  - Indexbildung
  - Modellierung und Simulation
    
* Software
  - [ArcGis](https://www.esri.de/produkte/arcgis)
  - [QGis](https://www.qgis.org/de/site/)
  - [R](https://www.r-project.org/)
    - [R und OSM](https://dominicroye.github.io/en/2018/accessing-openstreetmap-data-with-r/)

# Beispiel 
## Gesundheitsrelevante Daten
* Risikofaktoren
  - Gebaute Umwelt
    - Grünflächen
    - Wasserflächen
    - Waldflächen
    - Sportanlaagen
    - Schwimmbad
    - Spielplätze
    - Verkaufsstellen,
    - ÖPNV
    - Bewegungsfreundlichkeit der Wohnumgebung Walkability
    - Straßennetz
    - Einwohnerdichte
    - Landnutzung
    - Bodenbedeckung
  - Physische Umwelt
    - Luftverschmutzung
    - Lärmbelastung
    - Hitzebelastung
  - Soziale Umwelt
    - Merkmale der regionalen Deprivation
* Versorgung 
  - Ambulante Versorgung
    - Hausärzte
    - Fachärzte
    - Apotheken
  - Stationäre Versorgung
    - Krankenhäuser

## Vorgehen
1. Geodaten erschließen
2. Geodaten aufbereiten
  - Objekte aus Datensatz extrahieren
  - Objekte bearbeiten
3. Indikatoren berechnen
  - Z.B. Verfügbarkeit / Erreichbarkeit bestimmter Objekte
  - Z.B. Bewegungsfreundlichkeit der Verkehrsinfrastruktur
4. Indikatoren an einen Survey-Datensatz anspielen
5. Analysen durchführen

## Routing
* Die tatsächliche Entfernung anstelle von Luftlinie berechnen


# Fazit
- Steigende Aufmerksamkeit
- Präzise und standardisierte Datenerfassung
- Zusäztliche Imformationen zu den Risiko- und Schutzfaktoren
- Auswertung auf Gemeindeebene für einige Fragestellung nicht kleinräumig genug
- Geodaten können einen Beitrag für die Planung und Durchführung von Surveys leisten  