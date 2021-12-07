---
title: тип ресурса chatRenamedEventMessageDetail
description: Представляет сведения о сообщении события о переименовании чата.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4969a9c165dc957bafd832890597fe58e9629a2d
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322594"
---
# <a name="chatrenamedeventmessagedetail-resource-type"></a>тип ресурса chatRenamedEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о переименовании [чата.](../resources/chat.md)
Это сообщение создается при обновлении группы или темы чата собраний. 


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|chatDisplayName|Строка|Обновленное имя **чата.**|
|chatId|Строка|Уникальный идентификатор **чата.**|
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
- [Пример ответа на сообщение события о переименовании **чата**](/graph/system-messages/#chat-renamed)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
