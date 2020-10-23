---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6057c8cf71ce0f8d71632267d3790c39b69b1eb1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735766"
---
# <a name="aaduserconversationmember-resource-type"></a>Тип ресурса aadUserConversationMember

Пространство имен: microsoft.graph

Представляет пользователя Azure Active Directory в [команде](team.md).
Этот тип наследуется от [conversationMember](conversationmember.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление участников](../api/conversationmember-list.md) | Коллекция [conversationMember](conversationmember.md) | Получение списка всех пользователей в чате или канале.|
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

