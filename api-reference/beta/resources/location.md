---
title: Тип ресурса Location
description: Представляет сведения о месте проведения события.
localization_priority: Normal
ms.openlocfilehash: 6e3c61bcf8f22a20bf41053c2310dc51f5b800a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508610"
---
# <a name="location-resource-type"></a>Тип ресурса Location

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о месте проведения [мероприятия](event.md).

Создавать события в календаре можно несколькими способами, например с помощью REST API [создания события](../api/user-post-events.md) в приложении либо вручную с помощью пользовательского интерфейса Outlook. Создавая событие через пользовательский интерфейс, вы можете указать место проведения обычным текстом (например, "Бар «Окунь»") или выбрать его из списка помещений, предоставленного приложением Outlook, [Автозаполнением Bing](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) или [локальным поиском Bing](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/). 

В зависимости от того, как создано событие, Outlook может по-разному задавать доступное только для чтения свойство **locationType**. 

| Способ создания события  | Свойство   | Ожидаемое значение |
|:----------|:-------|:--------------------------------|
| REST API [создания события](../api/user-post-events.md) | **locationType** | `default` |
| Пользовательский интерфейс Outlook | **locationType** | Одно из следующих значений: <ul><li>`default` для расположения, указанного обычным текстом;</li><li>`conferenceRoom` для помещения из списка в Outlook;</li><li>любое из значений `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness` и `postalAddress` для расположения из Автозаполнения Bing или локального поиска Bing.</li></ul> |




## <a name="properties"></a>Свойства
| Свойство  | Тип   | Описание                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| address | [physicalAddress](physicaladdress.md) |Почтовый адрес расположения. |
| coordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | Географические координаты и высота расположения. |
| displayName  | String | Имя, связанное с расположением.                       |
| locationEmailAddress | String | Необязательный электронный адрес для расположения. |
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
<!--
{
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/location.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
