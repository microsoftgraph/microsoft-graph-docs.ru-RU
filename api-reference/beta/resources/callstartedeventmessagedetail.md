---
title: тип ресурса callStartedEventMessageDetail
description: Представляет сведения о сообщении события о запущенных вызовах.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: de887904a352749b2a8edd3e9b4d5554e0f34d49
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534331"
---
# <a name="callstartedeventmessagedetail-resource-type"></a>тип ресурса callStartedEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события о запущенных вызовах.
Это сообщение создается при вызове.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|callEventType|teamworkCallEventType|Представляет тип события вызова. Возможные значения: `call`, `meeting`, `screenShare`, `unknownFutureValue`.|
|callId|Строка|Уникальный идентификатор вызова.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callStartedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callStartedEventMessageDetail",
  "callId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "callEventType": "String"
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о запущенных вызовах](/graph/system-messages/#call-started)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)