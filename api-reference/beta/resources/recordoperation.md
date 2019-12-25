---
title: Тип ресурса Рекордоператион
description: Содержит сведения, связанные с записью звука.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 837540c55bb6573828efe87ee0c7ae333335ea11
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870140"
---
# <a name="recordoperation-resource-type"></a>Тип ресурса Рекордоператион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения, связанные с записью звука.

## <a name="properties"></a>Свойства

| Свойство                       | Тип                        | Описание                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| Контекст                  | String                      | Уникальная строка контекста клиента. Максимальный лимит — 256 символов.                                                                                                                               |
| комплетионреасон               | String                      | Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`. |
| id                             | Строка                      | ИДЕНТИФИКАТОР операции сервера. Только для чтения.                                                                                              |
| рекордингакцесстокен           | String                      | Маркер доступа, необходимый для получения записи.                                                                                              |
| рекординглокатион              | String                      | Расположение, в котором находится запись.                                                                                                      |
| resultInfo                     | [resultInfo](resultinfo.md) | Сведения о результате.  Только для чтения.                                                                                              |
| status                         | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения.                                                |

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
