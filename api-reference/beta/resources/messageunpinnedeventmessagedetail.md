---
title: Тип ресурса messageUnpinnedEventMessageDetail
description: Представляет сведения о сообщении о событии о незакрепленных сообщениях чата.
author: sumanac
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 28cdd335bf2d11d934782f5f94d359865b5b5b50
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118688"
---
# <a name="messageunpinnedeventmessagedetail-resource-type"></a>Тип ресурса messageUnpinnedEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о событии сообщения о [незакрепленной записи chatMessage](../resources/chatmessage.md). Это сообщение создается при откреплении сообщения чата.

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
  "@odata.type": "microsoft.graph.messageUnpinnedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.messageUnpinnedEventMessageDetail",
  "eventDateTime": "String (timestamp)",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение о событии о незакрепленном сообщении чата](/graph/system-messages/#message-unpinned)
- Дополнительные сведения о других типах событий см. в [разделе "Системные сообщения"](/graph/system-messages).
