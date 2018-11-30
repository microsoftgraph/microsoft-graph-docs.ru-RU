---
title: Тип ресурса onenoteOperation
description: Состояние определенных операций OneNote, выполняющихся в течение длительного времени.
ms.openlocfilehash: 913562abf1d2f644bd621268c93768c7500f4399
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028384"
---
# <a name="onenoteoperation-resource-type"></a>Тип ресурса onenoteOperation

Состояние определенных операций OneNote, выполняющихся в течение длительного времени.

## <a name="json-representation"></a>Представление в формате JSON

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
|error|[onenoteOperationError](onenoteoperationerror.md)|Ошибка при выполнении операции.|
|id|строка|Идентификатор операции. Только для чтения.|
|lastActionDateTime| DateTimeOffset |Время последнего действия операции.|
|resourceId|строка|Идентификатор ресурса.|
|resourceLocation|string|URI ресурса для объекта. Например, URI ресурса для скопированной страницы или раздела. |
|status|string|Текущее состояние операции: `notstarted`, `running`, `completed`, `failed`. |
|percentComplete|string|Процент завершения операции, если операция в состоянии `running`.

## <a name="relationships"></a>Связи
Нет


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение операции](../api/onenoteoperation-get.md) | [onenoteOperation](onenoteoperation.md) |Получение состояния операции. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
