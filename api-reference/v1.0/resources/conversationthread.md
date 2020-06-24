---
title: Тип ресурса conversationThread
description: conversationThread — это коллекция экземпляров post.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 8608ea72c8c136b54f94c73f99ca0f79fbc7ec0b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845269"
---
# <a name="conversationthread-resource-type"></a>Тип ресурса conversationThread

Пространство имен: microsoft.graph

conversationThread — это коллекция экземпляров [post](post.md).

The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients.
A new thread is created when a recipient is removed from the thread.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление цепочек](../api/group-list-threads.md) | Коллекция [conversationThread](conversationthread.md) |Получение всех цепочек группы.|
|[Создание цепочки](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.|
|[Получение conversationThread](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |Получение определенной цепочки, принадлежащей группе. |
|[Обновление](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |Обновление объекта conversationThread. |
|[Удаление](../api/conversationthread-delete.md) | Нет |Удаление объекта conversationThread. |
|[Ответ](../api/conversationthread-reply.md)|Нет|Создание ответа для этой цепочки с помощью создания сущности Post.|
|[Список сущностей Post](../api/conversationthread-list-posts.md) |Коллекция [post](post.md)| Получение записей для указанной цепочки. |

## <a name="properties"></a>Свойства
| Свойство              | Тип                                 | Описание                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    | String                               | Только для чтения.                                                                                                                                                                                       |
| toRecipients          | Коллекция [recipient](recipient.md) | Получатели в поле "Кому" для цепочки.                                                                                                                                                               |
| ccRecipients          | Коллекция [recipient](recipient.md) | Получатели в поле "Копия" для цепочки.                                                                                                                                                               |
| topic                 | String                               | The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.                                                                              |
| hasAttachments        | Boolean                              | Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение.                                                                                                               |
| ластделивереддатетиме | DateTimeOffset                       | The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'` |
| уникуесендерс         | Коллекция String                    | Все пользователи, которые отправили сообщение в эту цепочку.                                                                                                                                                |
| preview               | String                               | Краткая сводка из тела последней публикации в этой беседе.                                                                                                                           |
| isLocked              | Boolean                              | Указывает, заблокирована ли цепочка.                                                                                                                                                               |

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|posts|Коллекция [post](post.md)| Read-only. Nullable.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationThread",
  "@odata.annotations": [
    {
      "property": "posts",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
