---
title: тип ресурса callTranscriptEventMessageDetail
description: Представляет сведения о сообщении события о расшифровке вызовов.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a57a6f5fc98fb518cf55d56c784fb86ec4c8aab
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322606"
---
# <a name="calltranscripteventmessagedetail-resource-type"></a>тип ресурса callTranscriptEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о расшифровке вызовов.
Это сообщение создается, когда транскрипция доступна для вызова.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|callId|Строка|Уникальный идентификатор вызова.|
|callTranscriptICalUid|Строка|Уникальный идентификатор для расшифровки вызовов.|
|meetingOrganizer|[identitySet](../resources/identityset.md)|Организатор собрания.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callTranscriptEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callTranscriptEventMessageDetail",
  "callId": "String",
  "callTranscriptICalUid": "String",
  "meetingOrganizer": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о расшифровке вызовов](/graph/system-messages/#call-transcript)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
