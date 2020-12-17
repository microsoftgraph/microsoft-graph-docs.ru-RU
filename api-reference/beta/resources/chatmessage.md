---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте канала или чата. Сообщение чата может быть корневым сообщением чата или частью потока, определенного **свойством replyToId** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: b942cfe5c4a1ca08c201a2f51f9178d5db592413
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705838"
---
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md). Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.

> **Примечание.** Этот ресурс поддерживает подписку на изменения (создание, обновление и удаление) с помощью [уведомлений об изменениях.](../resources/webhooks.md) Это позволяет вызывающим подписаться на изменения и получать их в режиме реального времени. Дополнительные сведения см. в разделе [Получение уведомлений о сообщениях](/graph/teams-changenotifications-chatMessage).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Сообщения канала**| | |
|[Список каналов chatMessage](../api/channel-list-messages.md) | Коллекция [chatMessage](chatmessage.md) | Список всех сообщений корневого чата в канале.|
|[Get chatMessages in a channel delta](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Получать добавонные сообщения чата в канале. |
|[Создание подписки для новых сообщений канала](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Прослушивайте новые и измененные сообщения канала и реакции на них. |
|[Get channel chatMessage](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | Получите одно корневое сообщение чата из канала.|
|[Создание chatMessage в канале или чате](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| Создайте новое сообщение чата верхнего уровня в канале.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление свойства **policyViolation** сообщения чата.|
|**Ответы на сообщения канала**| | |
|[Список ответов на chatMessage](../api/channel-list-messagereplies.md) | Коллекция [chatMessage](chatmessage.md)| Список всех ответов на сообщение чата в канале.|
|[Получить ответ на chatMessage](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| Получите один ответ на сообщение чата в канале.|
|[Ответ на chatMessage в канале](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| Ответ на существующее сообщение чата в канале.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление свойства **policyViolation** сообщения чата.|
|**1:1 и сообщения группового чата**| | |
|[Get chatMessage in chat](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Получить одно сообщение чата в чате. |
|[Список chatMessages в чате](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | Список сообщений чата в 1:1 или групповом чате. |
|[Создание подписки для новых сообщений чата](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Прослушивайте новые и измененные сообщения чата и реакции на них. |
|[Создание chatMessage в чате](../api/chat-post-message.md) | [chatMessage](chatmessage.md)| Отправка сообщения чата в существующей беседе 1:1 или групповом чате.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление свойства **policyViolation** сообщения чата.|
|**Hosted content**| | |
|[Список всего ведущего контента](../api/chatmessage-list-chatmessagehostedcontents.md) | [Коллекция chatMessageHostedContent](../resources/chatmessagehostedcontent.md)| Получить все содержимое в сообщении чата.|
|[Get hosted content](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | Получать содержимое, которое вы можете получить из сообщения чата.|


## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|replyToId| string | Только для чтения. ИД родительского сообщения чата или сообщения корневого чата потока. (Применяется только к сообщениям чата в каналах, а не к чатам.) |
|from|[identitySet](identityset.md)| Только для чтения. Сведения об отправителю сообщения чата.|
|etag| string | Только для чтения. Номер версии сообщения чата. |
|messageType|string|Тип сообщения чата. Возможные значения: `message` .|
|createdDateTime|dateTimeOffset|Только для чтения. Timestamp of when the chat message was created.|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Timestamp when the chat message is created (initial setting) or modified, including when a reaction is added or removed. |
|lastEditedDateTime|dateTimeOffset|Только для чтения. Timestamp when edits to the chat message were made. Вызывает флаг "Изменено" в пользовательском интерфейсе Teams. Если изменения не внося, значение `null` будет .|
|deletedDateTime|dateTimeOffset|Только для чтения. Timestamp at which the chat message was deleted, or null if not deleted. |
|subject|string| Тема сообщения чата в обычном текстовом тексте.|
|body|[itemBody](itembody.md)|Представление содержимого сообщения чата в формате Plaintext/HTML. Представление определяется параметром contentType в тексте. Содержимое всегда находится в ФОРМАТЕ HTML, если сообщение чата содержит [chatMessageMention.](chatmessagemention.md) |
|summary|string| Сводный текст сообщения чата, который можно использовать для push-уведомлений и сводных представлений или отсвещенных представлений. Применяется только к сообщениям чата канала, а не к чатам в чате. |
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Вложенные файлы. В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается. |
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностями, упомянутыми в сообщении чата. В настоящее время поддерживаются значения user, bot, team и channel.|
|importance|string | Важность сообщения чата. Допустимые значения: `normal`, `high`, `urgent`.|
|reactions| Коллекция [chatMessageReaction](./chatmessagereaction.md) | Реакции на это сообщение чата (например, "Нравится").|
|языковые стандарты|string|Региональные региональные органы сообщения чата, установленного клиентом.|
| policyViolation | [chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md) |Определяет свойства нарушения политики, задав приложение защиты от потери данных (DLP).|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->


```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
  "deleted": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
