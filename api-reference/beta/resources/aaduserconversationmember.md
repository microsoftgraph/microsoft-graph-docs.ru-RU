---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 058164d44ef6d9d6ba6667cf1cb7249bf57c2a83
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633512"
---
# <a name="aaduserconversationmember-resource-type"></a>Тип ресурса aadUserConversationMember

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя Azure Active Directory в [чате](chat.md) или [канале](channel.md). Этот тип наследуется от [conversationMember](conversationmember.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление участников](../api/conversationmember-list.md) | Коллекция [conversationmember](conversationmember.md) | Получение списка всех пользователей в чате или канале.|
|[Получение участника](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | Получение одного пользователя в чате или канале.|
|[Добавление участника](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| Добавление участника в канал.|
|[Обновление участника](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| Обновление участника в канале.|
|[Удаление участника](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| Удаление участника из канала.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор пользователя.|
|displayName| string | Отображаемое имя пользователя. |
|roles| Коллекция строк | Роли этого пользователя. |
|userId| строка | GUID пользователя. |
|email| строка  | Электронный адрес пользователя. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
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
