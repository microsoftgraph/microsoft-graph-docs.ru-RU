---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fe5b7c324a478ef399147a3d12370842ae368632
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081785"
---
# <a name="aaduserconversationmember-resource-type"></a>Тип ресурса aadUserConversationMember

Пространство имен: microsoft.graph

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


