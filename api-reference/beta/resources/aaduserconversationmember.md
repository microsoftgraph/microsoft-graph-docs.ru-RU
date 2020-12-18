---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f19c5a2b711ab6c39069364c641066f1d9c6dbf
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705970"
---
# <a name="aaduserconversationmember-resource-type"></a>Тип ресурса aadUserConversationMember

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя Azure Active Directory в [чате](chat.md) или [канале](channel.md). Этот тип наследуется от [conversationMember](conversationmember.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список участников группы](../api/team-list-members.md)|Коллекция [conversationMember](../resources/conversationmember.md)|Получение списка участников группы.|
|[Получение участника группы](../api/team-get-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение участника группы.|
|[Добавление участника в команду](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|Добавление нового участника в группу.|
|[Массовое добавление участников в группу](../api/conversationmembers-add.md)|Коллекция [actionResultPart](../resources/actionresultpart.md)|Добавление нескольких участников в команду одним запросом.|
|[Обновление роли участника команды](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|Перевод пользователя из категории участников в категорию владельцев или наоборот, из категории владельцев в категорию обычных участников.|
|[Удаление участника группы](../api/team-delete-members.md)|Нет|Удаление существующего участника из группы.|
|[Перечисление участников канала](../api/channel-list-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех участников канала.|
|[Получение участника канала](../api/channel-get-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение участника канала.|
|[Создание участника канала](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | Добавление участника в канал. Поддерживается только для `channel` с типом членства `private`.|
|[Обновление роли участника канала](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | Обновление свойства участника канала. Поддерживается только для канала с типом членства `private`.|
|[Удаление участника канала](../api/channel-delete-members.md) | Нет | Удаление участника канала. Поддерживается, только если параметру `channelType` присвоено значение `private`.|
|[Перечисление участников чата](../api/chat-list-members.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех участников чата.|
|[Получение участника чата](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | Получение участника чата.|
|[Добавление участника в чат](../api/chat-post-members.md) | Заголовок размещения | Добавление участника в чат.| 

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id| String | Только для чтения. Уникальный идентификатор пользователя.|
|displayName| String | Отображаемое имя пользователя. |
|roles| Набор строк | Роли этого пользователя. |
|userId| String | GUID пользователя. |
|email| String  | Электронный адрес пользователя. |
|tenantId| string  | ИД клиента, которому принадлежит пользователь Azure AD. |
|visibleHistoryStartDateTime| DateTimeOffset  | Метка времени, обозначающая, насколько глубоко участник беседы может видеть историю беседы. Это свойство можно задать только для участников чата.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aadUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)",
  "userId": "String",
  "email": "String",
  "tenantId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
