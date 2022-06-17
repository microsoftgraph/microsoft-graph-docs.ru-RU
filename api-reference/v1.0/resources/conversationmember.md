---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
ms.localizationpriority: medium
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 299c98d0e751e835861fda43216c2bdabed05e24
ms.sourcegitcommit: 2132198551c7d1f37474debab471f612a3e35a08
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2022
ms.locfileid: "66141231"
---
# <a name="conversationmember-resource-type"></a>Тип ресурса conversationMember

Пространство имен: microsoft.graph

Представляет пользователя в команде, [канале](team.md) или [чате](chat.md).[](channel.md)
См. [также aadUserConversationMember](aaduserconversationmember.md).

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
|[Перечисление участников чата](../api/chat-list-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех участников чата.|
|[Добавление участника в чат](../api/chat-post-members.md) | Заголовок размещения | Добавление участника в чат.| 
|[Получение участника чата](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | Получение участника чата.|
|[Удаление участника чата](../api/chat-delete-members.md) | Нет | Удаление участника из чата.| 

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор пользователя.|
|displayName| string | Отображаемое имя пользователя. |
|roles| Коллекция строк | Роли этого пользователя. Это свойство содержит только дополнительные квалификаторы, если это необходимо. Например, `owner` если член имеет  привилегии, `owner` свойство ролей содержит одно из значений. Аналогично, если член является гостевым, свойство **ролей** содержит `guest` одно из значений. Базовый член не должен иметь значений, указанных в **свойстве** ролей.  |
|visibleHistoryStartDateTime| DateTimeOffset | Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы. Это свойство можно задать только для участников чата. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)"
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

