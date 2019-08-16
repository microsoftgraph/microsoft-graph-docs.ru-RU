---
title: Тип ресурса conversationMember
description: Представляет пользователя в беседе.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca5115922dfb40239b8ca290a39f3c5953d4e4ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973978"
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

## <a name="relationships"></a>Связи

Нет

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