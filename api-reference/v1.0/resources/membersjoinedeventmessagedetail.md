---
title: тип ресурса membersJoinedEventMessageDetail
description: Представляет сведения о сообщении о событиях, к участникам присоединились.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bbcbabbdec89c44aa88adbae36191472fee31053
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322570"
---
# <a name="membersjoinedeventmessagedetail-resource-type"></a>тип ресурса membersJoinedEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении о событиях, к участникам [присоединились.](../resources/conversationMember.md)
Это сообщение создается, когда **участники присоединяются** к чату [собраний.](../resources/chat.md)


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|members|[коллекция teamworkUserIdentity](../resources/teamworkuseridentity.md)|Список **участников, присоединившихся** к **чату.**|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.membersJoinedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.membersJoinedEventMessageDetail",
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
- [Пример ответа на сообщение о событиях, в которые **присоединились участники**](/graph/system-messages/#members-joined)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
