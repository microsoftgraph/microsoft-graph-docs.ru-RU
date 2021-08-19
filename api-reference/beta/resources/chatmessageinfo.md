---
title: тип ресурса chatMessageInfo
description: Представляет предварительный просмотр ресурса chatMessage.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 289bce30b970edd46f0ad29fdbaa24fd6428c93d
ms.sourcegitcommit: 6f04ad0e0cde696661511dcdf343942b43f73fc6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "58397042"
---
# <a name="chatmessageinfo-resource-type"></a>тип ресурса chatMessageInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет предварительный просмотр [ресурса chatMessage.](../resources/chatmessage.md) Этот объект может быть извлечен только в составе списка [чатов.](../resources/chat.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|body|[itemBody](../resources/itembody.md)|Тело [chatMessage](../resources/chatmessage.md). Это будет по-прежнему содержать маркеры для @mentions и вложений, даже если объект не возвращает @mentions и вложения.|
|createdDateTime|DateTimeOffset|Объект времени даты, представляющий время создания сообщения.|
|from|[chatMessageFromIdentitySet](../resources/chatmessagefromidentityset.md)|Сведения о отправителье сообщения.|
|id|Строка|ID [chatMessage](../resources/chatmessage.md).|
|isDeleted|Логический|Если `true` установлено, исходное сообщение удалено.|
|messageType|chatMessageType|Тип сообщения чата. Допустимые значения: `message`, `unknownFutureValue`, `systemEventMessage`.|
|eventDetail|[eventMessageDetail](../resources/eventmessagedetail.md)|Только для чтения.  При этом представлены сведения о событии, произошедшем в чате, канале или группе, например, добавлены участники и так далее. Для сообщений событий будет установлено свойство **messageType** `systemEventMessage` .|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageInfo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageInfo",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "from": {
    "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
  },
  "createdDateTime": "String (timestamp)",
  "isDeleted": "Boolean",
  "messageType": "String",
  "eventDetail": {
    "@odata.type": "microsoft.graph.eventMessageDetail"
  }
}
```

## <a name="see-also"></a>См. также

- [chat](../resources/chat.md)
- [chatMessage](../resources/chatmessage.md)

