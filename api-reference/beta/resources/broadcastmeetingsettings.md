---
title: Тип ресурса broadcastMeetingSettings
description: Параметры, связанные с трансляцией
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 42ac666817b6f259dd888e479939216fc3e39c6c
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866254"
---
# <a name="broadcastmeetingsettings-resource-type"></a>Тип ресурса broadcastMeetingSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры, связанные с трансляцией.

> [!IMPORTANT]
> Этот API не проверяет параметры трансляций, управляемые [политикой.](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell)
> Например, если администратор задает политику трансляций с помощью, пользователям будет запрещено устанавливать разрешения трансляций в клиенте Teams, но они смогут создавать трансляции с помощью Microsoft Graph, задав для `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany` `public` **allowedAudience** параметр `everyone` . 

## <a name="properties"></a>Свойства

| Свойство                   | Тип                     | Описание                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| allowedAudience            | broadcastMeetingAudience | Определяет, кто может присоединиться к трансляции. Возможные значения перечислены в следующей таблице. |
| isRecordingEnabled         | Логический                  | Указывает, включена ли запись для этого трансляции. Значение по умолчанию: `false`.          |
| isAttendeeReportEnabled    | Логический                  | Указывает, включен ли отчет участника для этого трансляции. Значение по умолчанию: `false`.    |
| isQuestionAndAnswerEnabled | Логический                  | Указывает, включен ли вопрос&A для этого трансляции. Значение по умолчанию: `false`.                |
| isVideoOnDemandEnabled     | Логический                  | Указывает, включено ли видео по требованию для этого трансляции. Значение по умолчанию: `false`.    |

### <a name="broadcastmeetingaudience-values"></a>Значения broadcastMeetingAudience

| Значение              | Описание                                                       |
| ------------------ | ----------------------------------------------------------------- |
| все           | Трансляция будет открыта для всех. Это значение используется по умолчанию. |
| organization;       | Все в вашей организации могут присоединиться к трансляции.                     |
| roleIsAttendee     | Только указанные люди могут присоединиться к трансляции.                |
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
