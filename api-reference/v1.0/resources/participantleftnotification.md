---
title: тип ресурса participantLeftNotification
description: Содержит сведения о участнике, основанном на политике, который покинул вызов.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b0b74588d4014b53b79ec43adfd37443b52d60334319b8e126e1deccafb9dcd2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141394"
---
# <a name="participantleftnotification-resource-type"></a>тип ресурса participantLeftNotification

Пространство имен: microsoft.graph

Содержит сведения о участнике, основанном на политике, который покинул вызов.

В [сценарии](/microsoftteams/teams-recording-policy) записи на основе политики, когда участник, управляемый вызовом бота, покинул собрание, боту будет отправлено уведомление бота с сведениями о событии, оставленного `participantLeftNotification` участником.

## <a name="properties"></a>Свойства
| Свойство       | Тип            | Описание                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| call           | [call](call.md) | Объект вызова, содержащий сведения о событии присоединения участника. |
| participantId  | String          | ID участника в соответствии с политикой, которая покинула собрание.        |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantLeftNotification"
}-->
```json
{
  "participantId": "String",
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantLeftNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
