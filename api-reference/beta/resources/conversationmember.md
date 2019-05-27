---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: f6908106390e527ab4e33e777dd232b58ead727a
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379306"
---
# <a name="conversationmember-resource-type"></a>Тип ресурса conversationMember

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя в [чате](chat.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список участников чата](../api/conversationmember-list.md) | Коллекция [conversationmember](conversationmember.md) | Получение списка всех пользователей в чате.|
|[Получение участника чата](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | Получение одного пользователя в чате.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор пользователя.|
|displayName| string | Отображаемое имя пользователя. |
|roles| Коллекция строк | Роли этого пользователя. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"]
}

```

## <a name="see-also"></a>См. также

[aadUserConversationMember](aaduserconversationmember.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
