---
title: Тип ресурса aadUserConversationMember
description: Представляет пользователя Azure Active Directory в чате или канале.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d53709726c55cc3ac9f2051bd499a996b33d9c36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028359"
---
# <a name="aaduserconversationmember-resource-type"></a>Тип ресурса aadUserConversationMember

Пространство имен: microsoft.graph

Представляет пользователя Azure Active Directory в [команде](team.md).
Этот тип наследуется от [conversationMember](conversationmember.md).

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

