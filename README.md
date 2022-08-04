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
      }
    },
      "geometry": {
        "type": "MultiPolygon",
        "coordinates": [
          [
            [
              [-83.682201, 10.935602]
            ]
          ]
        ]
      }
}
```

## Sobre zonas_postales.json

El formato del JSON contiene la siguiente estructura:

```json
{
	'[REGION]': {
		'[ESTADO]': {
			'iso_3166_2':'[CODIGO ISO_3166-2]',
			'[MUNICIPIO]': {
				'[PARROQUIA]': {
					'zonas': {
						'[ZONA]': [CODIGO_POSTAL], ...
					},
					'ciudad': [CIUDAD],
					'urbana': true|false
				}, ...
			}, ...
		}, ...
	}, ...
}
```
