---
title: Тип ресурса Намедлокатион
description: Это базовый класс, представляющий имя расположения Azure Active Directory. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fda5c1854dee5e6ce108f2cc46b95c6a69c64230
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089315"
---
# <a name="namedlocation-resource-type"></a>Тип ресурса Намедлокатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Это базовый класс, представляющий имя расположения Azure Active Directory. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Намедлокатионс](../api/conditionalaccessroot-list-namedlocations.md) | Коллекция [намедлокатион](namedLocation.md) | Получение всех объектов **намедлокатион** в Организации. |
| [Получение Намедлокатион](../api/namedlocation-get.md) | [намедлокатион](namedlocation.md) | Чтение свойств и связей объекта **намедлокатион** . |
| [Удаление Намедлокатион](../api/namedlocation-delete.md) | Нет | Удаление объекта **намедлокатион** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|displayName|Строка|Удобное для человека имя расположения.|
|id|Строка|Идентификатор объекта Намедлокатион. Только для чтения.|
|modifiedDateTime|DateTimeOffset|Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
  "baseType": "",
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


