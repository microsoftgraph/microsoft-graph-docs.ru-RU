---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d2e44349f7896dfed0d0dff455e9afd0ac65772
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714279"
---
# <a name="conversationmember-resource-type"></a>Тип ресурса conversationMember

Пространство имен: microsoft.graph

Представляет пользователя в команде, [канале](channel.md)или [чате.](chat.md) [](team.md)
См. [также aadUserConversationMember.](aaduserconversationmember.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список участников группы](../api/team-list-members.md)|Коллекция [conversationMember](../resources/conversationmember.md)|Получение списка участников группы.|
|[Добавление участника в команду](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|Добавление нового участника в группу.|
|[Получение участника группы](../api/team-get-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение участника группы.|
|[Обновление роли участника команды](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.|
|[Удаление участника группы](../api/team-delete-members.md)|Нет|Удаление существующего участника из группы.|
|[Перечисление участников канала](../api/channel-list-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех участников канала.|
|[Добавление участника канала](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | Добавление участника в канал. Поддерживается только для `channel` с типом членства `private`.|
|[Получение участника канала](../api/channel-get-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение участника канала.|
|[Обновление роли участника канала](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | Обновление свойства участника канала. Поддерживается только для канала с типом членства `private`.|
|[Удаление участника канала](../api/channel-delete-members.md) | Нет | Удаление участника канала. Поддерживается, только если параметру `channelType` присвоено значение `private`.|

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

