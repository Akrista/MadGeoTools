# Utileria de Estados, Municipios, Parroquias, Códigos Postales y Códigos ISO-3166-2.

Este fork contiene un agregado para los estados donde se utiliza el código ISO-3166-2. ISO 3166-2 es la segunda parte del estándar internacional de normalización ISO 3166, publicado por la Organización Internacional de Normalización (ISO), que define los códigos de identificación de las principales subdivisiones (por ejemplo, provincias o estados) de todos los países codificados en ISO 3166-1.

## Sobre el contenido del Repositorio

- zonas_postales.pdf - Fuente de donde se obtuvieron los Códigos Postales de Venezuela (IPOSTEL)
- zonas_postales.json - Parser del PDF de Ipostel en formato JSON
- zonas_postales.csv - Parser del PDF de Ipostel en formato CSV
- zonas_postales.csv - Parser del PDF de Ipostel en formato XLSX
- zonas_postales.sql - Parser del PDF de Ipostel en formato SQL

La data contiene:

- 35086 Zonas
- 1132 Parroquias
- 997 Ciudades
- 335 Municipios
- 24 Estados

## Sobre los Autores

Creado por Kijam López B. Desarrollador de https://cuado.co/ y http://kijam.com/.
Codigo ISO-3166-2 para Venezuela agregado por por Jorge Thomas https://linktr.ee/akrista.

## Sobre el Uso y Licencia

Todo el contenido publicado se puede editar, distribuir y utilizar solo bajo los términos de la Licencia GPLv3 - Ver GPL.md

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
