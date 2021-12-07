---
title: membersDeletedEventMessageDetail resource type
description: Представляет сведения о сообщении события об удаленных членах.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0f33dfa80fc27f7eb48e00dbaa6c427f7bb30a45
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322671"
---
# <a name="membersdeletedeventmessagedetail-resource-type"></a>membersDeletedEventMessageDetail resource type

Пространство имен: microsoft.graph

Представляет сведения о сообщении события об [удаленных](../resources/conversationMember.md) членах.
Это сообщение создается **при** удалении участников из чата, [](../resources/chat.md) [канала](../resources/channel.md)или [команды.](../resources/team.md)


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|members|[коллекция teamworkUserIdentity](../resources/teamworkuseridentity.md)|Список **удаленных** участников.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersDeletedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersDeletedEventMessageDetail",
  "members": [
    {
      "@odata.type": "microsoft.graph.teamworkUserIdentity"
    }
  ],
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события об **удаленных** членах](/graph/system-messages/#members-deleted)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
