---
title: тип ресурса participantJoiningNotification
description: Содержит сведения о присоединении участника, основанного на политике, к вызову.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e915697ba01e8968d7833e8701eaf1914984c28f
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430860"
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
