---
title: Тип ресурса onenoteOperation
description: Состояние определенных длительно выполняемых операций OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 9e427776d1a001ad3be9badca2dd731c2b42a057
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039207"
---
# <a name="onenoteoperation-resource-type"></a>Тип ресурса onenoteOperation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Состояние определенных длительно выполняемых операций OneNote.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
|error|[оненотеоператионеррор](onenoteoperationerror.md)|Ошибка, возвращенная операцией.|
|id|string|Идентификатор операции. только для чтения.|
|ластактиондатетиме| DateTimeOffset |Время последнего действия операции.|
|resourceId|string|Идентификатор ресурса.|
|ресаурцелокатион|string|URI ресурса для объекта. Например, URI ресурса для скопированной страницы или раздела. |
|status|string|Текущее состояние операции: `notstarted` ,, `running` `completed` , `failed` |
|percentComplete|string|Процент завершения операции, если операция все еще находится в `running` состоянии.

## <a name="relationships"></a>Отношения
Нет


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение операции](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |Получение состояния операции. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


