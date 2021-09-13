---
title: тип ресурса broadcastMeetingSettings
description: Параметры, связанные с событием в прямом эфире
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0a78c4665c42bf11c983bbf24aa72a93cdff323a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59031717"
---
# <a name="broadcastmeetingsettings-resource-type"></a>тип ресурса broadcastMeetingSettings

Пространство имен: microsoft.graph

Параметры, связанных с живым событием.

## <a name="properties"></a>Свойства

| Свойство                   | Тип                                                         | Описание                                                                                 |
|----------------------------|--------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| allowedAudience            | [broadcastMeetingAudience](#broadcastmeetingaudience-values) | Определяет, кто может присоединиться к событию в прямом эфире. Возможные значения перечислены в следующей таблице.     |
| isRecordingEnabled         | Логический                                                      | Указывает, включена ли запись для этого события в прямом эфире. Значение по умолчанию — `false`.       |
| isAttendeeReportEnabled    | Boolean                                                      | Указывает, включен ли отчет участника для этого события в прямом эфире. Значение по умолчанию — `false`. |
| isQuestionAndAnswerEnabled | Boolean                                                      | Указывает, включен ли Q&A для этого события в прямом эфире. Значение по умолчанию — `false`.             |
| isVideoOnDemandEnabled     | Логический                                                      | Указывает, включено ли видео по запросу для этого события в прямом эфире. Значение по умолчанию — `false`. |

### <a name="broadcastmeetingaudience-values"></a>значения broadcastMeetingAudience

| Значение              | Описание                                                       |
|--------------------|-------------------------------------------------------------------|
| все           | Событие в прямом эфире будет открыто для всех. Это значение используется по умолчанию. |
| organization;       | Все в вашей организации могут присоединиться к событию в прямом эфире.                     |
| roleIsAttendee     | Только указанные люди могут присоединиться к событию в прямом эфире.                |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать.                 |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "allowedAudience": "everyone | organization | roleIsAttendee | unknownFutureValue",
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
