---
title: тип ресурса broadcastMeetingSettings
description: Параметры, связанные с событием в прямом эфире
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f199a82ee90d6848cb68d670d49d7af1c1d2c739
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944116"
---
# <a name="broadcastmeetingsettings-resource-type"></a>тип ресурса broadcastMeetingSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры, связанные с живым событием.

> [!CAUTION]
> Этот API не проверяет параметры событий в прямом эфире, управляемые [политикой.](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell)
> Например, если администратор задает политику событий в прямом эфире с помощью, пользователям будет запрещено устанавливать разрешения на живые события в клиенте Teams, но он сможет создать живое событие с помощью `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany` `public` Microsoft Graph,  `everyone` установив разрешенное разрешение на .

## <a name="properties"></a>Свойства

| Свойство                   | Тип                     | Описание                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | Определяет, кто может присоединиться к событию в прямом эфире. Возможные значения перечислены в следующей таблице. |
| isRecordingEnabled         | Boolean                  | Указывает, включена ли запись для этого события в прямом эфире. Значение по умолчанию — `false`.          |
| isAttendeeReportEnabled    | Boolean                  | Указывает, включен ли отчет участника для этого события в прямом эфире. Значение по умолчанию — `false`.    |
| isQuestionAndAnswerEnabled | Boolean                  | Указывает, включен ли Q&A для этого события в прямом эфире. Значение по умолчанию — `false`.                |
| isVideoOnDemandEnabled     | Boolean                  | Указывает, включено ли видео по запросу для этого события в прямом эфире. Значение по умолчанию — `false`.    |

### <a name="broadcastmeetingaudience-values"></a>значения broadcastMeetingAudience

| Значение              | Описание                                                       |
| ------------------ | ----------------------------------------------------------------- |
| все           | Событие в прямом эфире будет открыто для всех. Это значение используется по умолчанию. |
| organization;       | Все в вашей организации могут присоединиться к событию в прямом эфире.                     |
| roleIsAttendee     | Только указанные люди могут присоединиться к событию в прямом эфире.                |
| unknownFutureValue | Неизвестное будущее значение.                                             |

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
