---
title: Тип ресурса Чатмессажехостедконтент
description: Контент, размещенный в сообщении чата
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2787138819160a25d72fb9ed273950eee326399c
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720971"
---
# <a name="chatmessagehostedcontent-resource-type"></a>Тип ресурса Чатмессажехостедконтент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контент, размещенный в сообщении чата, например изображения или фрагменты кода.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Чатмессажехостедконтент](../api/chatmessagehostedcontent-get.md) | [Чатмессажехостедконтент](chatmessagehostedcontent.md) | Чтение свойств и связей объекта **чатмессажехостедконтент** . |

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
