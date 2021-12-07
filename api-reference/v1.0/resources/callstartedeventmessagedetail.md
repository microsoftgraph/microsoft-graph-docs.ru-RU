---
title: тип ресурса callStartedEventMessageDetail
description: Представляет сведения о сообщении события о запущенных вызовах.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2e567a4dae25ff671b86c78a03243c93ddcf9e90
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322540"
---
# <a name="callstartedeventmessagedetail-resource-type"></a>тип ресурса callStartedEventMessageDetail

Пространство имен: microsoft.graph

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
