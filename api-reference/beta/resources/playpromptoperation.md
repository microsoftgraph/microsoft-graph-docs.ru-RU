---
title: Тип ресурса playPromptOperation
description: Операция playPrompt для получения результатов playPrompt действие.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: bc18b8f64dedd3fa4d758778bbee37c6bcfd46c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814380"
---
# <a name="playpromptoperation-resource-type"></a>Тип ресурса playPromptOperation

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Операция playPrompt для получения результатов playPrompt действие.

## <a name="properties"></a>Свойства

| Свойство            | Тип                        | Описание|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | Строка                      | Контекст клиента.                                                                |
| completionReason    | Строка                      | Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`. |
| createdDateTime     | DateTimeOffset              | Время начала операции.                                                   |
| id                  | Строка                      | Только для чтения.                                                                         |
| lastActionDateTime  | DateTimeOffset              | Время последнего действия операции.                                      |
| resultInfo          | [resultInfo](resultInfo.md) | Сведения о результатов. Только для чтения. Сервер, созданный.                               |
| status              | Строка                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`.               |

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
