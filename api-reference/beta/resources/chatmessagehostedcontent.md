---
title: Тип ресурса Чатмессажехостедконтент
description: Контент, размещенный в сообщении чата
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 39939d9d61d992e5fd77fd21360ab05e8f83dbd4
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333365"
---
# <a name="chatmessagehostedcontent-resource-type"></a>Тип ресурса Чатмессажехостедконтент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контент, размещенный в сообщении чата, например изображения или фрагменты кода.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Чатмессажехостедконтент](../api/chatmessage-list-chatmessagehostedcontents.md) | [чатмессажехостедконтент](chatmessagehostedcontent.md) | Получение списка **чатмессажехостедконтент** для сообщения. |
| [Получение Чатмессажехостедконтент](../api/chatmessagehostedcontent-get.md) | [чатмессажехостедконтент](chatmessagehostedcontent.md) | Чтение свойств и связей объекта **чатмессажехостедконтент** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
