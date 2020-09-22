---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d9e50c0ca27843461b41b4d86f29ce3604788866
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016769"
---
# <a name="conversationmember-resource-type"></a>Тип ресурса conversationMember

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя в [чате](chat.md) или [канале](channel.md).
См. также [аадусерконверсатионмембер](aaduserconversationmember.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список участников чата](../api/conversationmember-list.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех пользователей в чате.|
|[Получение участника чата](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | Получение одного пользователя в чате.|
|[Список участников](../api/conversationmember-list.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех пользователей в чате или канале.|
|[Получение участника](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | Получение одного пользователя в чате или канале.|
|[Добавление участника](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| Добавление участника в канал.|
|[Обновление участника](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| Обновление участника в канале.|
|[Удаление участника](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| Удаление участника из канала.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор пользователя.|
|displayName| string | Отображаемое имя пользователя. |
|roles| Коллекция строк | Роли этого пользователя. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


