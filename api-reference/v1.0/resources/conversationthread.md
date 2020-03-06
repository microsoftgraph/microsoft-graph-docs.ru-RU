---
title: Тип ресурса conversationThread
description: conversationThread — это коллекция экземпляров post.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 4e49e8617125758f606c42c47de3d9d13495666f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531757"
---
# <a name="conversationthread-resource-type"></a>Тип ресурса conversationThread

Пространство имен: Microsoft. Graph A conversationThread — это коллекция [posts](post.md).

Коллекция получателей последней записи — это все получатели для цепочки. Коллекция получателей для цепочки может увеличиваться. При удалении получателя из цепочки создается новая цепочка.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление цепочек](../api/group-list-threads.md) | Коллекция [conversationThread](conversationthread.md) |Получение всех цепочек группы.|
|[Создание цепочки](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |Создание беседы путем создания цепочки. В группе создаются беседа, цепочка беседы и запись.|
|[Получение conversationThread](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |Получение определенной цепочки, принадлежащей группе. |
|[Обновление](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |Обновление объекта conversationThread. |
|[Удаление](../api/conversationthread-delete.md) | Нет |Удаление объекта conversationThread. |
|[Ответ](../api/conversationthread-reply.md)|Нет|Создание ответа для этой цепочки с помощью создания сущности Post.|
|[Список сущностей Post](../api/conversationthread-list-posts.md) |Коллекция [post](post.md)| Получение записей для указанной цепочки. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели в поле "Кому" для цепочки.|
|ccRecipients|Коллекция [recipient](recipient.md)|Получатели в поле "Копия" для цепочки.|
|topic|String|Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.||
|hasAttachments|Boolean|Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение.|
|ластделивереддатетиме|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|уникуесендерс|Коллекция String|Все пользователи, которые отправили сообщение в эту цепочку.|
|preview|Строка|Краткая сводка из текста последней записи в этой беседе.|
|isLocked|Boolean|Указывает, заблокирована ли цепочка.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|posts|Коллекция [post](post.md)| Только для чтения. Допускается значение null.|

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
