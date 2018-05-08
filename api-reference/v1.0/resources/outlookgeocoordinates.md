# <a name="outlookgeocoordinates-resource-type"></a>Тип ресурса outlookGeoCoordinates

Географические координаты, высота и точность физического местоположения.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|accuracy|double|Точность широты и долготы. Например, точность может измеряться в метрах и составлять 50 метров.|
|altitude|double|Высота местоположения.|
|altitudeAccuracy|double|Точность высоты.|
|latitude|double|Широта местоположения.|
|longitude|double|Долгота местоположения.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->