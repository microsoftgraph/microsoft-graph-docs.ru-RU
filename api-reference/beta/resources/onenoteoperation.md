---
title: Тип ресурса onenoteOperation
description: Состояние определенных операций OneNote, выполняющихся в течение длительного времени.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 146a1b1d9a51cc541e06fd789f987a2d39dff48a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512852"
---
# <a name="onenoteoperation-resource-type"></a>Тип ресурса onenoteOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Состояние определенных операций OneNote, выполняющихся в течение длительного времени.

## <a name="json-representation"></a>Представление в формате JSON

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
|error|[onenoteOperationError](onenoteoperationerror.md)|Ошибка при выполнении операции.|
|id|string|Идентификатор операции. Только для чтения.|
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
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
