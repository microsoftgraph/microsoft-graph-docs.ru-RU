---
title: membersAddedEventMessageDetail resource type
description: Представляет сведения о добавленных членах сообщения события.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: df1bb119f115d047fb8d5ff6a426ae259d8fe55d
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322653"
---
# <a name="membersaddedeventmessagedetail-resource-type"></a>membersAddedEventMessageDetail resource type

Пространство имен: microsoft.graph

Представляет сведения о добавленных членах сообщения [события.](../resources/conversationMember.md)
Это сообщение создается при **добавлении** участников в [чат,](../resources/chat.md) [канал](../resources/channel.md)или [команду.](../resources/team.md)
Свойство **visibleHistoryStartDateTime** для события  о членах, добавленных в канал, всегда задано, что указывает, что вся история является  `0001-01-01T00:00:00Z` общей.

> **Примечание.**  Свойство **visibleHistoryStartDateTime** для [conversationMember](conversationmember.md) и сообщения **membersAddedEventMessageDetail** может иметь разные значения, если выбранное  значение **shareHistoryTime** для участников в чате раньше видимого времени истории инициатора.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|members|[коллекция teamworkUserIdentity](../resources/teamworkuseridentity.md)|Список **добавленных** участников.|
|visibleHistoryStartDateTime|DateTimeOffset|Timestamp, который обозначает, как далеко назад история беседы совместно с участниками беседы.|

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
- [Пример ответа на сообщение события о **добавленных членах**](/graph/system-messages/#members-added)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
