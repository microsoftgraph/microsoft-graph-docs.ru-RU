---
title: тип ресурса meetingPolicyUpdatedEventMessageDetail
description: Представляет сведения о сообщении события об обновленной политике собраний.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 256f50d33957ca76bdeedda604698c80739b431b
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322547"
---
# <a name="meetingpolicyupdatedeventmessagedetail-resource-type"></a>тип ресурса meetingPolicyUpdatedEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события об обновленной политике собраний.
Это сообщение создается при обновлении **параметра Разрешить собрание** чат.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|meetingChatEnabled|Boolean|Представляет, включен ли [чат](../resources/chat.md) собрания или нет.|
|meetingChatId|Строка|Уникальный идентификатор чата **собраний.**|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingPolicyUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingPolicyUpdatedEventMessageDetail",
  "meetingChatId": "String",
  "meetingChatEnabled": "Boolean",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение о событии об обновленной политике собраний](/graph/system-messages/#meeting-policy-updated)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
