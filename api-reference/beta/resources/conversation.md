---
title: Тип ресурса conversation
description: Беседа — коллекция цепочек, содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 038ec9dd7abe0dfc5b9ef7eeda1c6d1837f4e1db
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513029"
---
# <a name="conversation-resource-type"></a>Тип ресурса conversation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Беседа — коллекция [цепочек](conversationthread.md), содержащих записи. Все цепочки и записи в беседе имеют одинаковую тему.

Этот ресурс поддерживает подписку на изменение [уведомлений.](/graph/webhooks)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление бесед](../api/group-list-conversations.md) | Коллекция [conversation](conversation.md) |Получение списка бесед в этой группе.|
|[Создание](../api/group-post-conversations.md) |[conversation](conversation.md)| Создание беседы путем включения цепочки и записи.|
|[Получение беседы](../api/conversation-get.md) | [conversation](conversation.md) |Считывание свойств и отношений объекта conversation.|
|[удаление](../api/conversation-delete.md); | Нет |Удаление объекта conversation. |
|[Список цепочек беседы](../api/conversation-list-threads.md) |Коллекция [conversationThread](conversationthread.md)| Получение всех цепочек в групповой беседе.|
|[Создание цепочки беседы](../api/conversation-post-threads.md) |Коллекция [conversationThread](conversationthread.md)| Создание цепочки в указанной беседе.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|hasAttachments|Boolean|Указывает, содержит ли какая-либо запись в этой беседе хотя бы одно вложение. Поддерживает `$filter` `eq` (, `ne` ) и `$search` .|
|id|Строка|Уникальный идентификатор беседы. Только для чтения.|
|lastDeliveredDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Поддерживает `$filter` (`eq`, `ne`, `le`, `ge`).|
|preview|String|Краткая сводка из тела последней публикации в этом разговоре.|
|topic|String|Тема беседы. Это свойство можно задать при создании беседы, но его невозможно обновить.|
|uniqueSenders|Коллекция String|Все пользователи, которые отправили сообщение в эту беседу.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|threads|Коллекция [conversationThread](conversationthread.md)|Коллекция всех цепочек в беседе. Свойство навигации. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


