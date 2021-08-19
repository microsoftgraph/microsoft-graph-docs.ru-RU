---
title: тип ресурса countryNamedLocation
description: Представляет расположение Azure Active Directory, определенное странами и регионами. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 28a00add81da2c755e81704052aa04774e5a0baf
ms.sourcegitcommit: 6f04ad0e0cde696661511dcdf343942b43f73fc6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396755"
---
# <a name="countrynamedlocation-resource-type"></a>тип ресурса countryNamedLocation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|countriesAndRegions|Коллекция String|Список стран и/или регионов в формате двух букв, заданный ISO 3166-2.|
|countryLookupMethod|countryLookupMethodType|Определяет, какой метод используется для определения страны, в которой находится пользователь. Возможные значения: `clientIpAddress` и `authenticatorAppGps`. Примечание. `authenticatorAppGps` Еще не поддерживается в Microsoft Cloud for US Government.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. Наследуется [от namedLocation](../resources/namedLocation.md).|
|displayName|Строка|Понятное человеку имя расположения. Наследуется [от namedLocation](../resources/namedLocation.md).|
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
  "countryLookupMethod": "countryLookedupMethodType",
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


