---
title: Тип ресурса messagePinnedEventMessageDetail
description: Представляет сведения о сообщении о событии о закрепленных сообщениях чата.
author: sumanac
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: acec5aaf817549c6ac4913b2aced914ee6a497d2
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118682"
---
# <a name="messagepinnedeventmessagedetail-resource-type"></a>Тип ресурса messagePinnedEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении о событии закрепленного [chatMessage](../resources/chatmessage.md). Это сообщение создается при закреплении сообщения чата.

Наследуется [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|eventDateTime|DateTimeOffset|Дата и время возникновения события.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.messagePinnedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.messagePinnedEventMessageDetail",
  "eventDateTime": "String (timestamp)",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение о событии о закрепленном сообщении чата](/graph/system-messages/#message-pinned)
- Дополнительные сведения о других типах событий см. в [разделе "Системные сообщения"](/graph/system-messages).
