---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 663675bb895d452c9ad50c89f22f1a51efca20a9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536997"
---
# <a name="playpromptoperation-resource-type"></a>Тип ресурса Плайпромптоператион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Операция Плайпромпт для получения результата действия Плайпромпт.

## <a name="properties"></a>Свойства

| Свойство            | Тип                        | Описание|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| Контекст       | String                      | Контекст клиента.                                                                |
| Комплетионреасон    | String                      | Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`. |
| createdDateTime     | DateTimeOffset              | Время начала операции.                                                   |
| id                  | Строка                      | Только для чтения.                                                                         |
| Ластактиондатетиме  | DateTimeOffset              | Время последнего действия операции.                                      |
| resultInfo          | [resultInfo](resultinfo.md) | Сведения о результате. Только для чтения. Создается сервером.                               |
| status              | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`.               |

## <a name="relationships"></a>Отношения
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
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
