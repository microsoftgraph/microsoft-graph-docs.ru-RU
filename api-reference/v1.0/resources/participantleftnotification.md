---
title: тип ресурса participantLeftNotification
description: Содержит сведения о участнике, основанном на политике, который покинул вызов.
author: yizhenww
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cdd3bb5b41fcd37c03b1814e7226ce84e6edafa1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036055"
---
# <a name="participantleftnotification-resource-type"></a>тип ресурса participantLeftNotification

Пространство имен: microsoft.graph

Содержит сведения о участнике, основанном на политике, который покинул вызов.

В [сценарии](/microsoftteams/teams-recording-policy) записи на основе политики, когда участник, управляемый вызовом бота, покинул собрание, боту будет отправлено уведомление бота с сведениями о событии, оставленного `participantLeftNotification` участником.

## <a name="properties"></a>Свойства
| Свойство       | Тип            | Описание                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| call           | [call](call.md) | Объект вызова, содержащий сведения о событии присоединения участника. |
| participantId  | Строка          | ID участника в соответствии с политикой, которая покинула собрание.        |

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
