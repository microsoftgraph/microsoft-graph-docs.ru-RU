---
title: membersAddedEventMessageDetail resource type
description: Представляет сведения о добавленных членах сообщения события.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 33d0c73ff5726310c1a4566813bd034cd9d5e9cc
ms.sourcegitcommit: 6f04ad0e0cde696661511dcdf343942b43f73fc6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396993"
---
# <a name="membersaddedeventmessagedetail-resource-type"></a>membersAddedEventMessageDetail resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о добавленных членах сообщения события.
Это сообщение создается при добавлении участников в чат, канал или команду.
Свойство **visibleHistoryStartDateTime** для добавленного события участников в канале всегда задано, что указывает, что вся история `0001-01-01T00:00:00Z` является общей.

> **Примечание.** Для чата, когда выбранное время истории совместной работы для участников более раннее, чем видимое время истории инситатора, свойство **visibleHistoryStartDateTime** для [conversationMember](conversationmember.md) и сообщение **membersAddedEventMessageDetail** могут иметь разные значения. [conversationMember](conversationmember.md) имеет эффективное время видимой истории для участника на основе видимого времени истории инициатора.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|members|[коллекция teamworkUserIdentity](../resources/teamworkuseridentity.md)|Список добавленных участников.|
|visibleHistoryStartDateTime|DateTimeOffset|Timestamp, обозначающий, как далеко от истории беседы делятся с участниками беседы.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersAddedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersAddedEventMessageDetail",
  "members": [
    {
      "@odata.type": "microsoft.graph.teamworkUserIdentity"
    }
  ],
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "visibleHistoryStartDateTime": "String (timestamp)"
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о добавленных членах](/graph/system-messages/#members-added)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
