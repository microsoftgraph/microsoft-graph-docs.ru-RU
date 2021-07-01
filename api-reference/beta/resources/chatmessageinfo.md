---
title: тип ресурса chatMessageInfo
description: Представляет предварительный просмотр ресурса chatMessage.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dc03ee6743aa8115f5a231b3766cc2d6c3d5537b
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236318"
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
|id|String|ID [chatMessage](../resources/chatmessage.md).|
|isDeleted|Логический|Если `true` установлено, исходное сообщение удалено.|

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
  "isDeleted": "Boolean"
}
```

## <a name="see-also"></a>См. также

- [chat](../resources/chat.md)
- [chatMessage](../resources/chatmessage.md)

