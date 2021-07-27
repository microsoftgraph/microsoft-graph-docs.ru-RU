---
title: тип ресурса callTranscriptEventMessageDetail
description: Представляет сведения о сообщении события о расшифровке вызовов.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 00d5b1e4433cb74fdc1e0c023727a93cbd2ac54b
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534334"
---
# <a name="calltranscripteventmessagedetail-resource-type"></a>тип ресурса callTranscriptEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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