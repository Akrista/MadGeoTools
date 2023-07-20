# Utilerias para Georeferencias.

Este fork contiene un agregado para los estados donde se utiliza el código ISO-3166-2. ISO 3166-2 es la segunda parte del estándar internacional de normalización ISO 3166, publicado por la Organización Internacional de Normalización (ISO), que define los códigos de identificación de las principales subdivisiones (por ejemplo, provincias o estados) de todos los países codificados en ISO 3166-1.

Asi mismo, planeo agregar mas utilerias que pueda ayudar en gestiones relacionadas con Georeferencias en diferentes apps.

## Sobre el contenido del Repositorio

### **GeoJsons**

La inclusión de GeoJsons se debe a una necesidad surgida en el uso de la herramienta [ClicData](https://app.clicdata.com/help/docs) y la codificación necesaria para que esta herramienta pueda trabajar con GeoJsons.

- [ ] Regiones
  - [x] Latinoamerica
  - [x] Sudamerica
  - [x] Centroamerica
- [ ] Paises
  - [ ] Venezuela

### **Postal Zones**

- [x] zonas_postales.pdf - Fuente de donde se obtuvieron los Códigos Postales de Venezuela (IPOSTEL)
- [x] zonas_postales.json - Parser del PDF de Ipostel en formato JSON
- [x] zonas_postales.csv - Parser del PDF de Ipostel en formato CSV
- [x] zonas_postales.csv - Parser del PDF de Ipostel en formato XLSX
- [x] zonas_postales.sql - Parser del PDF de Ipostel en formato SQL

La data contiene:

- 35086 Zonas
- 1132 Parroquias
- 997 Ciudades
- 335 Municipios
- 24 Estados

## Fuentes de Datos

Gran parte de los GeoJson han sido extraídos del Repo: https://github.com/codeforgermany/click_that_hood
<br>
Creado por Kijam López B. Desarrollador de https://cuado.co/ y http://kijam.com/.
<br>
Codigo ISO-3166-2 para Venezuela agregado por por Jorge Thomas https://linktr.ee/akrista.
<br>
GeoJson de Estados y Parroquias obtenido de [CENDITEL](https://mpv.cenditel.gob.ve/)

## Sobre el Uso y Licencia

Todo el contenido publicado se puede editar, distribuir y utilizar solo bajo los términos de la Licencia GPLv3 - Ver [Licencia](LICENSE)

## Sobre ClicData GeoJsons

Siguiendo la documentación de [ClicData](https://app.clicdata.com/help/docs/region-map-custom), el formato del GeoJson contiene la siguiente estructura:

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": {
        "iso_alpha3": "CRI",
        "name": "Costa Rica",
        "id": "CR",
        "cartodb_id": 4,
        "created_at": "2014-09-30T00:00:00Z",
        "updated_at": "2014-09-30T00:00:00Z"
      },
      "geometry": {
        "type": "MultiPolygon",
        "coordinates": [
          [
            [
              [-77.367774, 8.675762],
              [-77.447398, 8.472832],
              [-77.158488, 7.931887],
              [-77.563463, 7.507522],
              [-77.729057, 7.695723],
              [-77.702932, 7.457188],
              [-77.891671, 7.225743],
              [-78.445915, 8.055528],
              [-78.279999, 8.081722],
              [-78.164726, 8.399431],
              [-78.248413, 8.379861],
              [-78.418335, 8.551139],
              [-78.420998, 8.347445],
              [-78.515358, 8.638833],
              [-79.087448, 9.040472],
              [-79.584053, 8.976556],
              [-79.858696, 8.653389],
              [-79.751053, 8.598722],
              [-80.473389, 8.230778],
              [-79.99247, 7.516472],
              [-80.439003, 7.239944],
              [-80.89003, 7.205639],
              [-81.056221, 7.914889],
              [-81.222969, 7.884278],
              [-81.229057, 7.609083],
              [-81.51564, 7.709055],
              [-81.760719, 8.213528],
              [-82.718086, 8.326694],
              [-82.875053, 8.028139],
              [-83.052127, 8.331154],
              [-82.839001, 8.480281],
              [-82.919289, 8.765018],
              [-82.71189, 8.922495],
              [-82.936111, 9.07838],
              [-82.856184, 9.618039],
              [-82.342667, 9.432834],
              [-82.396637, 9.265139],
              [-82.170807, 9.195666],
              [-82.244919, 8.998305],
              [-81.789192, 8.943334],
              [-81.894836, 9.18825],
              [-81.546082, 8.823389],
              [-81.304276, 8.78],
              [-79.921555, 9.291056],
              [-79.624336, 9.6165],
              [-78.971001, 9.564722],
              [-79.060387, 9.439362],
              [-78.562637, 9.443306],
              [-78.038002, 9.235583],
              [-77.367774, 8.675762]
            ],
            [
              [-78.141464, 8.40487],
              [-78.157303, 8.419888],
              [-78.164726, 8.399431],
              [-78.141464, 8.40487]
            ],
            [
              [-78.141464, 8.40487],
              [-77.96328, 8.235917],
              [-78.058945, 8.424167],
              [-78.141464, 8.40487]
            ]
          ]
        ]
      }
    }
  ]
}
```

Ejemplo en Vista:

```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": {
        "iso_alpha3": "CRI",
        "name": "Costa Rica",
        "id": "CR",
        "cartodb_id": 4,
        "created_at": "2014-09-30T00:00:00Z",
        "updated_at": "2014-09-30T00:00:00Z"
      },
      "geometry": {
        "type": "MultiPolygon",
        "coordinates": [
          [
            [
              [-77.367774, 8.675762],
              [-77.447398, 8.472832],
              [-77.158488, 7.931887],
              [-77.563463, 7.507522],
              [-77.729057, 7.695723],
              [-77.702932, 7.457188],
              [-77.891671, 7.225743],
              [-78.445915, 8.055528],
              [-78.279999, 8.081722],
              [-78.164726, 8.399431],
              [-78.248413, 8.379861],
              [-78.418335, 8.551139],
              [-78.420998, 8.347445],
              [-78.515358, 8.638833],
              [-79.087448, 9.040472],
              [-79.584053, 8.976556],
              [-79.858696, 8.653389],
              [-79.751053, 8.598722],
              [-80.473389, 8.230778],
              [-79.99247, 7.516472],
              [-80.439003, 7.239944],
              [-80.89003, 7.205639],
              [-81.056221, 7.914889],
              [-81.222969, 7.884278],
              [-81.229057, 7.609083],
              [-81.51564, 7.709055],
              [-81.760719, 8.213528],
              [-82.718086, 8.326694],
              [-82.875053, 8.028139],
              [-83.052127, 8.331154],
              [-82.839001, 8.480281],
              [-82.919289, 8.765018],
              [-82.71189, 8.922495],
              [-82.936111, 9.07838],
              [-82.856184, 9.618039],
              [-82.342667, 9.432834],
              [-82.396637, 9.265139],
              [-82.170807, 9.195666],
              [-82.244919, 8.998305],
              [-81.789192, 8.943334],
              [-81.894836, 9.18825],
              [-81.546082, 8.823389],
              [-81.304276, 8.78],
              [-79.921555, 9.291056],
              [-79.624336, 9.6165],
              [-78.971001, 9.564722],
              [-79.060387, 9.439362],
              [-78.562637, 9.443306],
              [-78.038002, 9.235583],
              [-77.367774, 8.675762]
            ],
            [
              [-78.141464, 8.40487],
              [-78.157303, 8.419888],
              [-78.164726, 8.399431],
              [-78.141464, 8.40487]
            ],
            [
              [-78.141464, 8.40487],
              [-77.96328, 8.235917],
              [-78.058945, 8.424167],
              [-78.141464, 8.40487]
            ]
          ]
        ]
      }
    }
  ]
}
```

## Sobre zonas_postales.json

El formato del JSON contiene la siguiente estructura:

```json
{
  "REGION": {
    "ESTADO": {
      "iso_3166_2": "CODIGO ISO_3166-2",
      "MUNICIPIO": {
        "PARROQUIA": {
          "zonas": {
            "ZONA": "CODIGO_POSTAL"
          },
          "ciudad": "CIUDAD",
          "urbana": "true|false"
        }
      }
    }
  }
}
```
