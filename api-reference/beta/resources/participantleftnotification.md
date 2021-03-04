---
title: тип ресурса participantLeftNotification
description: Содержит сведения о участнике, основанном на политике, который покинул вызов.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2730cd68e8d7ff6c5c238caeaee91fb4a821c836
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447506"
---
# <a name="participantleftnotification-resource-type"></a>тип ресурса participantLeftNotification

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

