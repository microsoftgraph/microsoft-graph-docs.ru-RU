---
title: тип ресурса countryNamedLocation
description: Представляет расположение Azure Active Directory, определенное странами и регионами. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 531942e5026e2fc3d4d9ed3311d9130275d5a853
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443167"
---
# <a name="countrynamedlocation-resource-type"></a>тип ресурса countryNamedLocation

Пространство имен: microsoft.graph

Представляет расположение Azure Active Directory, определенное странами и регионами. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.

Наследует от [namedLocation](../resources/namedLocation.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список countryNamedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [коллекция countryNamedLocation](countryNamedLocation.md) | Получите все **объекты countryNamedLocation** в организации. |
| [Создание countryNamedLocation](../api/conditionalaccessroot-post-namedlocations.md) | [countryNamedLocation](countryNamedLocation.md) | Создание нового **объекта countryNamedLocation.** |
| [Get countryNamedLocation](../api/countrynamedlocation-get.md) | [countryNamedLocation](countrynamedlocation.md) | Ознакомьтесь с свойствами и отношениями **объекта countryNamedLocation.** |
| [Обновление countryNamedLocation](../api/countrynamedlocation-update.md) | [countryNamedLocation](countrynamedlocation.md) | Обновление **объекта countryNamedLocation.** |
| [Удаление countryNamedLocation](../api/countrynamedlocation-delete.md) | Нет | Удаление **объекта countryNamedLocation.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|countriesAndRegions|Коллекция строк|Список стран и/или регионов в формате двух букв, заданный ISO 3166-2.|
|countryLookupMethod|countryLookupMethodType|Определяет, какой метод используется для определения страны, в которой находится пользователь. Возможные значения: `clientIpAddress` и `authenticatorAppGps`.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. Наследуется [от namedLocation](../resources/namedLocation.md).|
|displayName|String|Понятное человеку имя расположения. Наследуется [от namedLocation](../resources/namedLocation.md).|
|id|String|Идентификатор объекта namedLocation. Только для чтения. Наследуется [от namedLocation](../resources/namedLocation.md).|
|includeUnknownCountriesAndRegions|Логический|Верно, если IP-адреса, которые не относятся к стране или региону, должны быть включены в именоваемом расположении.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет последнюю измененную дату и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. Наследуется [от namedLocation](../resources/namedLocation.md).|

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
  "countryLookupMethod": "String",
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
