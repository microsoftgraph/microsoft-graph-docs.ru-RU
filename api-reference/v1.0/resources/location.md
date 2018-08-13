# <a name="location-resource-type"></a>Тип ресурса Location

Представляет сведения о месте проведения [мероприятия](event.md).

Создавать события в календаре можно несколькими способами, например с помощью REST API [создания события](../api/user_post_events.md) в приложении либо вручную с помощью пользовательского интерфейса Outlook. Создавая событие через пользовательский интерфейс, вы можете указать место проведения обычным текстом (например, "Бар «Окунь»") или выбрать его из списка помещений, предоставленного приложением Outlook, [Автозаполнением Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) или [локальным поиском Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/). 

В зависимости от того, как создано событие, Outlook может по-разному задавать доступное только для чтения свойство **locationType**. 

| Способ создания события  | Свойство   | Ожидаемое значение |
|:----------|:-------|:--------------------------------|
| REST API [создания события](../api/user_post_events.md) | **locationType** | `default` |
| Пользовательский интерфейс Outlook | **locationType** | Одно из следующих значений: <ul><li>`default` для расположения, указанного обычным текстом;</li><li>`conferenceRoom` для помещения из списка в Outlook;</li><li>любое из значений `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness` и `postalAddress` для расположения из Автозаполнения Bing или локального поиска Bing.</li></ul> |

## <a name="properties"></a>Свойства
| Свойство  | Тип   | Описание                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| address | [physicalAddress](physicaladdress.md) |Почтовый адрес расположения. |
| coordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | Географические координаты и высота расположения. |
| displayName  | String | Имя, связанное с расположением.                       |
| locationEmailAddress | String | Необязательный электронный адрес для расположения.              |
| locationUri | String | Необязательный URI, представляющий местоположение. |
| locationType | String | Тип расположения. Возможные значения: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`. Только для чтения.|
| uniqueId | String | Только для внутреннего использования.|
| uniqueIdType | String | Только для внутреннего использования. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string",
  "locationType": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
