---
title: тип ресурса channelRenamedEventMessageDetail
description: Представляет сведения о сообщении события о переименовании канала.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ffe2ae896a0f313f08d5af32753c4806831575c
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535788"
---
# <a name="channelrenamedeventmessagedetail-resource-type"></a>тип ресурса channelRenamedEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события о переименовании канала.
Это сообщение создается при обновлении имени канала.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|channelDisplayName|Строка|Обновленное имя канала.|
|channelId|Строка|Уникальный идентификатор канала.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelRenamedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о переименовании канала](/graph/system-messages/#channel-renamed)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
