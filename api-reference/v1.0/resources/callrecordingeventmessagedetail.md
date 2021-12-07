---
title: тип ресурса callRecordingEventMessageDetail
description: Представляет сведения о сообщении события о записи вызовов.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b37d49f0b13aa9da1445f74b74011f3bdc129112
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322701"
---
# <a name="callrecordingeventmessagedetail-resource-type"></a>тип ресурса callRecordingEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о записи вызовов.
Это сообщение создается, когда начинается запись вызова.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|callId|String|Уникальный идентификатор вызова.|
|callRecordingDisplayName|Строка|Отображение имени для записи вызова.|
|callRecordingDuration|Длительность|Продолжительность записи вызова.|
|callRecordingStatus|callRecordingStatus|Состояние записи вызова. Возможные значения: `success`, `failure`, `initial`, `chunkFinished`, `unknownFutureValue`.|
|callRecordingUrl|Строка|URL-адрес записи вызовов.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|meetingOrganizer|[identitySet](../resources/identityset.md)|Организатор собрания.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecordingEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecordingEventMessageDetail",
  "callId": "String",
  "callRecordingDisplayName": "String",
  "callRecordingUrl": "String",
  "callRecordingDuration": "String (duration)",
  "callRecordingStatus": "String",
  "meetingOrganizer": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о записи вызовов](/graph/system-messages/#call-recording)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)

