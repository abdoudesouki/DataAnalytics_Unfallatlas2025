
# Projektbeschreibung

## Analyse tödlicher Verkehrsunfälle in Deutschland

### 1. Projektübersicht
In diesem Projekt werden **tödliche Verkehrsunfälle in Deutschland** mithilfe von Daten aus dem **Unfallatlas 2025** analysiert. Ziel ist es, zeitliche, regionale und verkehrsbezogene Muster zu identifizieren und mögliche Zusammenhänge zwischen verschiedenen Unfallmerkmalen zu untersuchen.

Der Schwerpunkt liegt auf der explorativen Datenanalyse (Exploratory Data Analysis, EDA) und der Visualisierung der Ergebnisse mit Python.

---
## 2. Zielsetzung

Das Hauptziel des Projekts ist es, anhand der Unfallatlas-Daten zu untersuchen, **wann, wo und unter welchen Bedingungen tödliche Verkehrsunfälle besonders häufig auftreten**.

Dabei sollen insbesondere folgende Fragestellungen beantwortet werden:

- An welchen **Wochentagen** ereignen sich die meisten tödlichen Verkehrsunfälle?
- Gibt es Unterschiede zwischen den einzelnen **Monaten**?
- Zu welchen **Tageszeiten** treten besonders viele tödliche Unfälle auf?
- Wie häufig waren Fahrräder, Pkw, Fußgänger, Motorräder und Güterkraftfahrzeuge an Verkehrsunfällen beteiligt? 
- Wie häufig treten die verschiedenen Verkehrsteilnehmergruppen – Fußgänger, Radfahrer, Pkw, Güterkraftfahrzeuge (Gkfz), Krafträder (Krad) und sonstige Verkehrsmittel (e.g. Bus, Tram etc) – gemeinsam in Verkehrsunfällen auf?
- Gibt es **regionale Unterschiede** zwischen Bundesländern?
- Lassen sich **räumliche Unfallhäufungen bzw. Hotspots** erkennen?
- Wie verteilen sich tödliche Unfälle auf **Tageslicht und Verkehrsteilnehmergruppen**?
- Gibt es Zusammenhänge zwischen **Wochentag, Tageszeit**?

## 3. Datengrundlage

Als Datengrundlage wird der **Unfallatlas 2025** verwendet. Der Datensatz enthält Informationen zu Verkehrsunfällen mit Personenschaden in Deutschland.

Für die Analyse werden ausschließlich **Unfälle mit Getöteten** betrachtet.

Besonders relevante Variablen sind:

| Variable | Bedeutung |
|---|---|
| `UJAHR` | Unfalljahr |
| `UMONAT` | Unfallmonat |
| `USTUNDE` | Unfallstunde |
| `UWOCHENTAG` | Wochentag des Unfalls |
| `UKATEGORIE` | Unfallkategorie |
| `IstRad` | Fahrrad |
| `IstPKW` | PKW |
| `IstFuss` | Fußgänger |
| `IstKrad` | Motorrad |
| `IstGkfz` | Güterkraftfahrzeug |

### Daten Quelle: 

- [Unfallatlas](https://unfallatlas.statistikportal.de/)

  - [CSV format](https://www.opengeodata.nrw.de/produkte/transport_verkehr/unfallatlas/Unfallorte2025_EPSG25832_CSV.zip)

  - [Schema Beschreibung](https://www.opengeodata.nrw.de/produkte/transport_verkehr/unfallatlas/DSB_Unfallatlas.pdf)

- [JSON Geo](https://naturalearth.s3.amazonaws.com/10m_cultural/)

- [Bundesländer Deutschland](https://geodata.ucdavis.edu/gadm/gadm4.1/json/)

- [Destasis Bevölkerung](https://www.destatis.de/EN/Themes/Society-Environment/Population/Current-Population/Tables/population-by-laender-basis-2022.html)
