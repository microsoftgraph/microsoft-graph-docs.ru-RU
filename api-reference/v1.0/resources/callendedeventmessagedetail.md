---
title: тип ресурса callEndedEventMessageDetail
description: Представляет сведения о сообщении события о завершаемом вызове.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9a441f7f3562f7f07db93764544ab419e46fa16f
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322713"
---
# <a name="callendedeventmessagedetail-resource-type"></a>тип ресурса callEndedEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о завершаемом вызове.
Это сообщение создается после окончания вызова.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|callDuration|Длительность|Продолжительность вызова.|
|callEventType|teamworkCallEventType|Представляет тип события вызова. Возможные значения: `call`, `meeting`, `screenShare`, `unknownFutureValue`.|
|callId|String|Уникальный идентификатор вызова.|
|callParticipants|[коллекция callParticipantInfo](../resources/callparticipantinfo.md)|Список участников зова.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callEndedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callEndedEventMessageDetail",
  "callId": "String",
  "callParticipants": [
    {
      "@odata.type": "microsoft.graph.callParticipantInfo"
    }
  ],
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "callDuration": "String (duration)",
  "callEventType": "String"
}
```

## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о завершаемом вызове](/graph/system-messages/#call-ended)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)

