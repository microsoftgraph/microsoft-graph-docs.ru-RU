---
title: Тип ресурса recordOperation
description: Тип recordOperation
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6b9deb566e5b527a9f20db69441fa96908212a38
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512509"
---
# <a name="recordoperation-resource-type"></a>Тип ресурса recordOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип recordOperation

## <a name="properties"></a>Свойства

| Свойство                       | Тип                        | Описание                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| ClientContext                  | String                      | Контекст клиента.                                                                                                                               |
| completionReason               | String                      | Возможные значения: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`. |
| createdDateTime                | DateTimeOffset              | Время создания записи.                                                                                                          |
| id                             | String                      | Идентификатор операции сервера. Только для чтения. Сервер, созданный.                                                                                             |
| lastActionDateTime             | DateTimeOffset              | Время последнего действия операции.                                                                                                     |
| recordResourceAccessToken      | String                      | Маркер доступа, необходимые для извлечения записи.                                                                                              |
| recordResourceLocation         | String                      | Расположение, где расположена записи.                                                                                                      |
| resultInfo                     | [resultInfo](resultinfo.md) | Сведения о результатов.  Только для чтения. Сервер, созданный.                                                                                             |
| status                         | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения. Сервер, созданный.                                                 |

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

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
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>Пример

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "status": "completed"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/recordoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
