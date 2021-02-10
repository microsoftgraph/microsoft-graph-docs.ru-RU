---
title: Тип ресурса namedLocation
description: Это базовый класс, который представляет именуемую позицию Azure Active Directory. Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ee4e415545ea2b67d189c0ee582d51c3ea779575
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161091"
---
# <a name="namedlocation-resource-type"></a>Тип ресурса namedLocation

Пространство имен: microsoft.graph

Это базовый класс, который представляет именуемую позицию Azure Active Directory. Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список namedLocations](../api/conditionalaccessroot-list-namedlocations.md) | [Коллекция namedLocation](namedLocation.md) | Получите все **объекты namedLocation** в организации. |
| [Получить namedLocation](../api/namedlocation-get.md) | [namedLocation](namedlocation.md) | Чтение свойств и связей объекта **namedLocation.** |
| [Удаление namedLocation](../api/namedlocation-delete.md) | Нет | Удаление объекта **namedLocation.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет дату и время создания расположения в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|displayName|String|Понятное человеку имя расположения.|
|id|String|Идентификатор объекта namedLocation. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип Timestamp представляет дату и время последнего изменения расположения в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "namedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

