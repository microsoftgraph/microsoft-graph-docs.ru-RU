---
title: тип ресурса meetingPolicyUpdatedEventMessageDetail
description: Представляет сведения о сообщении события об обновленной политике собраний.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2fb18c1275fe6b0d9979978a0d07b4247ddfcdce
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534383"
---
# <a name="meetingpolicyupdatedeventmessagedetail-resource-type"></a>тип ресурса meetingPolicyUpdatedEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события об обновленной политике собраний.
Это сообщение создается при обновлении **параметра Разрешить собрание** чат.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|meetingChatEnabled|Boolean|Представляет, включен ли чат собрания или нет.|
|meetingChatId|Строка|Уникальный идентификатор чата собраний.|

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