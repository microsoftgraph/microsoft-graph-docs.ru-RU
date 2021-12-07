---
title: тип ресурса membersLeftEventMessageDetail
description: Представляет сведения о сообщении о событиях, оставленных участниками.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7fd75e032e58a2254cc9f9965360c2d3a9327759
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322552"
---
# <a name="memberslefteventmessagedetail-resource-type"></a>тип ресурса membersLeftEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении о событиях, [оставленных участниками.](../resources/conversationMember.md)
Это сообщение создается, **когда участники покидают** чат [собраний.](../resources/chat.md)


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|members|[коллекция teamworkUserIdentity](../resources/teamworkuseridentity.md)|Список **участников,** которые покинули **чат.**|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersLeftEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersLeftEventMessageDetail",
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
- [Пример ответа на сообщение о событиях, **оставленных участниками**](/graph/system-messages/#members-left)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
