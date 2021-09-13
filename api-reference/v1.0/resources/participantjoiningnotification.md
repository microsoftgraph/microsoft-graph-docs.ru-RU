---
title: тип ресурса participantJoiningNotification
description: Содержит сведения о присоединении участника, основанного на политике, к вызову.
author: yizhenww
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9e9b0186035e055b06c99fe60a52ca1ff63dc5bc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036062"
---
# <a name="participantjoiningnotification-resource-type"></a>тип ресурса participantJoiningNotification

Пространство имен: microsoft.graph

Содержит сведения о присоединении участника, основанного на политике, к вызову.

В [сценарии](/microsoftteams/teams-recording-policy)записи на основе политики перед тем, как участник политики присоединяется к вызову, боту, связанному с политикой, которая имеет доступную емкость для обработки нового участника, будет `participantJoiningNotification` отправлено.

[УчастникJoiningResponse в](participantjoiningResponse.md) ответной нагрузке ожидается от бота.

## <a name="properties"></a>Свойства
| Свойство       | Тип            | Описание                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| call           | [call](call.md) | Объект вызова, содержащий сведения о событии присоединения участника. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantJoiningNotification"
}-->
```json
{
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantJoiningNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
