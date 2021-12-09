---
title: тип ресурса broadcastMeetingSettings
description: Представляет параметры, связанные с живым событием в Microsoft Teams.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ca268c18f97db7609522a3bc6578acfd94d3ef0e
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390838"
---
# <a name="broadcastmeetingsettings-resource-type"></a>тип ресурса broadcastMeetingSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры, связанные с живым [событием](/microsoftteams/teams-live-events/what-are-teams-live-events) в Microsoft Teams.

## <a name="properties"></a>Свойства

| Свойство                   | Тип                     | Описание                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | Определяет, кто может присоединиться к Teams в прямом эфире. Возможные значения перечислены в следующей таблице. |
| isRecordingEnabled         | Логический                  | Указывает, включена ли запись для этого Teams в прямом эфире. Значение по умолчанию — `false`.          |
| isAttendeeReportEnabled    | Логический                  | Указывает, включен ли отчет участника для этого Teams в прямом эфире. Значение по умолчанию — `false`.    |
| isQuestionAndAnswerEnabled | Логический                  | Указывает, включен ли Q&A для этого Teams в прямом эфире. Значение по умолчанию — `false`.                |
| isVideoOnDemandEnabled     | Логический                  | Указывает, включено ли видео по запросу для этого Teams в прямом эфире. Значение по умолчанию — `false`.    |

### <a name="broadcastmeetingaudience-values"></a>значения broadcastMeetingAudience

| Значение              | Описание                                                       |
| ------------------ | ----------------------------------------------------------------- |
| все           | Это Teams будет открыто для всех. Это значение используется по умолчанию. |
| organization       | Все в вашей организации могут присоединиться к этому Teams в прямом эфире.                     |
| roleIsAttendee     | Только указанные люди могут присоединиться к этому событию Teams в прямом эфире.                |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать.  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "allowedAudience": "String",
  "isRecordingEnabled": "Boolean",
  "isAttendeeReportEnabled": "Boolean",
  "isQuestionAndAnswerEnabled": "Boolean",
  "isVideoOnDemandEnabled": "Boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "broadcastSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
