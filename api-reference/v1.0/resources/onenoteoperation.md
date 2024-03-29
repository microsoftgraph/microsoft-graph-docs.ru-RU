---
title: тип ресурса onenoteOperation
description: Состояние некоторых длительных OneNote операций.
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: ef25b94bb02ffaf721e7861eecacdd37c4c85e9f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118042"
---
# <a name="onenoteoperation-resource-type"></a>тип ресурса onenoteOperation

Пространство имен: microsoft.graph

Состояние некоторых длительных OneNote операций.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |Время начала операции.|
|error|[onenoteOperationError](onenoteoperationerror.md)|Ошибка, возвращаемая операцией.|
|id|string|ID операции. Только для чтения.|
|lastActionDateTime| DateTimeOffset |Время последнего действия операции.|
|resourceId|string|ID ресурса.|
|resourceLocation|string|URI ресурса для объекта. Например, ресурс URI для скопированной страницы или раздела. |
|status|operationStatus|Текущий статус операции: `NotStarted` `Running` , , `Completed` `Failed` . |
|percentComplete|string|Если операция по-прежнему находится в состоянии, операция будет `running` завершена в процентах.|

## <a name="relationships"></a>Отношения
Нет


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получить операцию](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |Получите состояние операции. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

