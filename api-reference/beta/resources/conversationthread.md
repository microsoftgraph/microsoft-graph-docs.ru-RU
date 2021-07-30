---
title: Тип ресурса conversationThread
description: conversationThread — это коллекция экземпляров post.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: d73c84fec11ae4ee3bbf1d07b237b82fbfc6ddf7
ms.sourcegitcommit: b711aed8acc18512cf6591f4108ed5ddf05b649d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2021
ms.locfileid: "53660312"
---
# <a name="conversationthread-resource-type"></a>Тип ресурса conversationThread

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

conversationThread — это коллекция экземпляров [post](post.md).

Коллекция получателей последней записи — это все получатели для цепочки. Коллекция получателей для цепочки может увеличиваться. При удалении получателя из цепочки создается новая цепочка.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление цепочек](../api/group-list-threads.md) | Коллекция [conversationThread](conversationthread.md) |Получение всех цепочек группы.|
|[Создание цепочки](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |Создание беседы путем создания цепочки. В группе создаются беседа, цепочка беседы и запись.|
|[Получение conversationThread](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |Получение определенной цепочки, принадлежащей группе. |
|[Обновление](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |Обновление объекта conversationThread. |
|[Удаление](../api/conversationthread-delete.md) | Нет |Удаление объекта conversationThread. |
|[reply](../api/conversationthread-reply.md)|Нет|Создание ответа для этой цепочки с помощью создания сущности Post.|
|[Список сущностей Post](../api/conversationthread-list-posts.md) |Коллекция [post](post.md)| Получение записей для указанной цепочки. |

## <a name="properties"></a>Свойства
| Свойство              | Тип                                 | Описание                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    | String                               | Только для чтения. <br/><br/>Возвращается по умолчанию.                                                                                                                                                                                      |
| toRecipients          | Коллекция [recipient](recipient.md) | Получатели в поле "Кому" для цепочки. <br/><br/>Возвращается только с помощью оператора $select.                                                                                                                                                               |
| ccRecipients          | Коллекция [recipient](recipient.md) | Получатели в поле "Копия" для цепочки. <br/><br/>Возвращается только с помощью оператора $select.                                                                                                                                                              |
| topic                 | String                               | Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить. <br/><br/>Возвращается по умолчанию.                                                                              |
| hasAttachments        | Boolean                              | Указывает, содержит ли какая-либо запись в этой цепочке хотя бы одно вложение. <br/><br/>Возвращается по умолчанию.                                                                                                               |
| lastDeliveredDateTime | DateTimeOffset                       | Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. <br/><br/>Возвращается по умолчанию. |
| uniqueSenders         | Коллекция String                    | Все пользователи, которые отправили сообщение в эту цепочку. <br/><br/>Возвращается по умолчанию.                                                                                                                                                |
| preview               | String                               | Краткая сводка из тела последней публикации в этом разговоре. <br/><br/>Возвращается по умолчанию.                                                                                                                           |
| isLocked              | Boolean                              | Указывает, заблокирована ли цепочка. <br/><br/>Возвращается по умолчанию.                                                                                                                                                               |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|posts|Коллекция [post](post.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread"
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
<!--
{
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


