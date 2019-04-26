---
title: Тип ресурса onenoteOperation
description: Состояние определенных длительно выполняемых операций OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: f336021221cd86a45f8c5683a9736cc6f838a913
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341447"
---
# <a name="onenoteoperation-resource-type"></a>Тип ресурса onenoteOperation

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
|error|[Оненотеоператионеррор](onenoteoperationerror.md)|Ошибка, возвращенная операцией.|
|id|строка|Идентификатор операции. Только для чтения.|
|Ластактиондатетиме| DateTimeOffset |Время последнего действия операции.|
|resourceId|string|Идентификатор ресурса.|
|Ресаурцелокатион|string|URI ресурса для объекта. Например, URI ресурса для скопированной страницы или раздела. |
|status|string|Текущее состояние операции: `notstarted`, `running`,, `completed``failed` |
|percentComplete|string|Процент завершения операции, если операция все еще находится в `running` состоянии.

## <a name="relationships"></a>Связи
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
