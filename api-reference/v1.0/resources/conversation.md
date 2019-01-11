---
title: Тип ресурса conversation
description: Беседа — коллекция цепочек, содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.
localization_priority: Normal
ms.openlocfilehash: c1d4bdda7efebb890458be2146dc72cdb9c76389
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862960"
---
# <a name="conversation-resource-type"></a>Тип ресурса conversation

Беседа — коллекция [цепочек](conversationthread.md), содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.

Этот ресурс поддерживает подписки на [уведомления об изменении](/graph/webhooks).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список бесед](../api/group-list-conversations.md) | Коллекция [conversation](conversation.md) |Получение списка бесед в этой группе.|
|[Создание](../api/group-post-conversations.md) |[conversation](conversation.md)| Создание беседы путем включения цепочки и записи.|
|[Получение беседы](../api/conversation-get.md) | [conversation](conversation.md) |Считывание свойств и отношений объекта conversation.|
|[Удаление](../api/conversation-delete.md) | Нет |Удаление объекта conversation. |
|[Список цепочек беседы](../api/conversation-list-threads.md) |Коллекция [conversationThread](conversationthread.md)| Получение всех цепочек в групповой беседе.|
|[Создание цепочки беседы](../api/conversation-post-threads.md) |Коллекция [conversationThread](conversationthread.md)| Создание цепочки в указанной беседе.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|hasAttachments|Boolean|Указывает, содержит ли какая-либо запись в этой беседе хотя бы одно вложение.|
|id|String|Уникальный идентификатор беседы. Только для чтения.|
|lastDeliveredDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|preview|String|Краткая сводка из текста последней записи в этой беседе.|
|topic|String|Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.|
|uniqueSenders|Коллекция String|Все пользователи, которые отправили сообщение в эту беседу.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|threads|Коллекция [conversationThread](conversationthread.md)|Коллекция всех цепочек в беседе. Свойство навигации. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversation",
  "@odata.annotations": [
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"],

  "threads": [{"@odata.type": "microsoft.graph.conversationThread"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
