---
title: тип ресурса chatRenamedEventMessageDetail
description: Представляет сведения о сообщении события о переименовании чата.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a247dd16674a6f7d3173ea5f3f5383d8fd2d68e
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534453"
---
# <a name="chatrenamedeventmessagedetail-resource-type"></a>тип ресурса chatRenamedEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события о переименовании чата.
Это сообщение создается при обновлении группы или темы чата собраний.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|chatDisplayName|Строка|Обновленное имя чата.|
|chatId|Строка|Уникальный идентификатор чата.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatRenamedEventMessageDetail",
  "chatId": "String",
  "chatDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о переименовании чата](/graph/system-messages/#chat-renamed)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)