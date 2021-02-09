---
title: Тип ресурса countryNamedLocation
description: Представляет именуемую позицию Azure Active Directory, определяемую в странах и регионах. Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d61621a0cade0bcb479f19ffb0c29050f367401
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157724"
---
# <a name="countrynamedlocation-resource-type"></a>Тип ресурса countryNamedLocation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет именуемую позицию Azure Active Directory, определяемую в странах и регионах. Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.

Наследуется от [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список countryNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [коллекция countryNamedLocation](countryNamedLocation.md) | Получить все **объекты countryNamedLocation** в организации. |
| [Создание countryNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [countryNamedLocation](countryNamedLocation.md) | Создание объекта **countryNamedLocation.** |
| [Get countryNamedLocation](../api/countrynamedlocation-get.md) | [countryNamedLocation](countrynamedlocation.md) | Чтение свойств и связей объекта **countryNamedLocation.** |
| [Обновление countryNamedLocation](../api/countrynamedlocation-update.md) | [countryNamedLocation](countrynamedlocation.md) | Обновление объекта **countryNamedLocation.** |
| [Удаление countryNamedLocation](../api/countrynamedlocation-delete.md) | Нет | Удаление объекта **countryNamedLocation.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|countriesAndRegions|Коллекция String|Список стран и/или регионов в двухформатном формате, заданном в ISO 3166-2.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет дату и время создания расположения в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Наследуется [от namedLocation.](../resources/namedLocation.md)|
|displayName|String|Понятное человеку имя расположения. Наследуется [от namedLocation.](../resources/namedLocation.md)|
|id|String|Идентификатор объекта namedLocation. Только для чтения. Наследуется [от namedLocation.](../resources/namedLocation.md)|
|includeUnknownCountriesAndRegions|Boolean|Имеет true, если IP-адреса, которые не сопойдутся со странаю или регионом, должны быть включены в именоваемом расположении.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет дату и время последнего изменения расположения в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. Наследуется [от namedLocation.](../resources/namedLocation.md)|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation"
}-->

```json
{
  "countriesAndRegions": ["String"],
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "includeUnknownCountriesAndRegions": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "countryNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


