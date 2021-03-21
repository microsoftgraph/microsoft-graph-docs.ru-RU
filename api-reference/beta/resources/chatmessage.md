---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте канала или чата. Сообщение чата может быть корневым сообщением чата или частью потока, определяемого **свойством replyToId** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 529ae74cd59df20233317cbd27cb28d03c700409
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958825"
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
|[Список каналов chatMessage](../api/channel-list-messages.md) | Коллекция [chatMessage](chatmessage.md) | Список всех корневых сообщений чата в канале.|
|[Получить chatMessages в дельте канала](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Получите дополнительные сообщения чата в канале. |
|[Создание подписки для новых сообщений канала](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Слушайте новые и отредактированы сообщения канала и реакции на них. |
|[Get channel chatMessage](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | Получите одно корневое сообщение чата из канала.|
|[Создание chatMessage в канале или чате](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| Создание нового сообщения чата верхнего уровня в канале.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление **свойства policyViolation** сообщения чата.|
|**Ответы на сообщения канала**| | |
|[Ответы списка на chatMessage](../api/channel-list-messagereplies.md) | Коллекция [chatMessage](chatmessage.md)| Список всех ответов на сообщение чата в канале.|
|[Получить ответ на chatMessage](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| Получите один ответ на сообщение чата в канале.|
|[Ответ на chatMessage в канале](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| Ответ на существующее сообщение чата в канале.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление **свойства policyViolation** сообщения чата.|
|**1:1 и групповые сообщения чата**| | |
|[Получить chatMessage в чате](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Получите одно сообщение чата в чате. |
|[Список chatMessages в чате](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | Список сообщений чата в чате 1:1 или групповом чате. |
|[Получите все сообщения чата для пользователя](../api/chats-getallmessages.md)| [коллекция чатов](chat.md)| Получите сообщения из всех чатов, в которых пользователь является участником, включая чаты 1:1, групповые чаты и чаты собраний. |
|[Создание подписки для новых сообщений чата](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Слушайте новые и отредактированы сообщения чата и реакции на них. |
|[Создание chatMessage в чате](../api/chat-post-message.md) | [chatMessage](chatmessage.md)| Отправка сообщения чата в существующей беседе 1:1 или групповом чате.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление **свойства policyViolation** сообщения чата.|
|**Содержимое с хост-контентом**| | |
|[Список всего содержимого, на которое было организовано](../api/chatmessage-list-chatmessagehostedcontents.md) | [коллекция chatMessageHostedContent](../resources/chatmessagehostedcontent.md)| Получите все содержимое в сообщении чата.|
|[Получить контент с хост-контентом](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | Получите у себя содержимое из сообщения чата.|


## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|replyToId| string | Только для чтения. ID родительского сообщения чата или корневого сообщения чата потока. (Применяется только к чатам в каналах, а не к чатам.) |
|from|[identitySet](identityset.md)| Только для чтения. Сведения о отправителье сообщения чата.|
|etag| string | Только для чтения. Номер версии сообщения чата. |
|messageType|string|Тип сообщения чата. Возможные значения: `message` .|
|createdDateTime|dateTimeOffset|Только для чтения. Время создания сообщения чата.|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Timestamp, когда сообщение чата создается (начальный параметр) или изменено, в том числе при добавлении или удалении реакции. |
|lastEditedDateTime|dateTimeOffset|Только для чтения. Timestamp, когда были сделаны изменения в сообщении чата. Вызывает флаг "Отредактирован" в пользовательском интерфейсе Teams. Если изменение не выполнено, значение `null` .|
|deletedDateTime|dateTimeOffset|Только для чтения. Timestamp, при котором сообщение чата было удалено, или null, если не удалено. |
|subject|string| Тема сообщения чата в plaintext.|
|body|[itemBody](itembody.md)|Представление plaintext/HTML контента сообщения чата. Представление определяется параметром contentType в тексте. Содержимое всегда находится в HTML, если в сообщении чата [содержится chatMessageMention.](chatmessagemention.md) |
|summary|string| Сводный текст сообщения чата, который можно использовать для push-уведомлений и сводных представлений или отпадения представлений. Применяется только к сообщениям чата, а не к чатам в чате. |
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Вложенные файлы. В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается. |
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностями, упомянутыми в сообщении чата. В настоящее время поддерживаются значения user, bot, team и channel.|
|importance|string | Важность сообщения чата. Допустимые значения: `normal`, `high`, `urgent`.|
|reactions| Коллекция [chatMessageReaction](./chatmessagereaction.md) | Реакции на это сообщение чата (например, Like).|
|языковые стандарты|string|Локализовать сообщение чата, за набором клиентом.|
| policyViolation | [chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md) |Определяет свойства нарушения политики, установленные приложением для предотвращения потери данных (DLP).|
|chatId|string| Удостоверение чата, в котором было размещено сообщение.|
|channelIdentity | [channelIdentity](../resources/channelIdentity.md) | Идентификатор канала, в котором было размещено сообщение.|

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
  "chatId": "string",
  "channelIdentity": {"@odata.type": "microsoft.graph.channelIdentity"},
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
