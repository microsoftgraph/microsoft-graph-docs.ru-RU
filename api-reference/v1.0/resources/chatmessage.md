---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте канала или чата. Сообщение чата может быть корневым сообщением чата или частью потока, определяемого **свойством replyToId** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: 300d17e32114eece7e1af3f9ab57c8b3af370494
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732191"
---
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

Пространство имен: microsoft.graph

Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md). Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.

> **Примечание.** Этот ресурс поддерживает подписку на изменения (создание, обновление и удаление) с помощью [уведомлений об изменениях.](../resources/webhooks.md) Это позволяет вызывающим подписаться на изменения и получать их в режиме реального времени. Дополнительные сведения см. в разделе [Получение уведомлений о сообщениях](/graph/teams-changenotifications-chatMessage).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Сообщения канала**| | |
|[Список сообщений в канале](../api/channel-list-messages.md) | Коллекция [chatMessage](chatmessage.md) | Список всех корневых сообщений в канале.|
|[Получить дельту сообщений в канале](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Получение добавочных сообщений в канале. |
|[Создание подписки для новых сообщений канала](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Слушайте новые, измененные и удаленные сообщения и реакции на них. |
|[Получать сообщение в канале](../api/chatmessage-get.md) | [chatMessage](chatmessage.md) | Получите одно корневое сообщение в канале.|
|[Отправка сообщения в канале](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| Создание нового корневого сообщения в канале.|
|[Обновление сообщения в канале](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление **свойства policyViolation** сообщения чата.|
|**Ответы на сообщения канала**| | |
|[Список ответов на сообщение](../api/chatmessage-list-replies.md) | Коллекция [chatMessage](chatmessage.md)| Список всех ответов на сообщение чата в канале.|
|[Получить сообщение ответа в канале](../api/chatmessage-get.md) | [chatMessage](chatmessage.md) | Получите одно сообщение ответа в канале.|
|[Ответ на сообщение в канале](../api/chatmessage-post-replies.md) | [chatMessage](chatmessage.md)| Ответ на существующее сообщение чата в канале.|
|[Обновление сообщения ответа](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление **свойства policyViolation** сообщения чата.|
|**Сообщения чата**| | |
|[Список сообщений в чате](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Список сообщений чата в чате. |
|[Получение сообщения в чате](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Получите одно сообщение чата в чате. |
|[Создание подписки для новых сообщений чата](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Слушайте новые, измененные и удаленные сообщения чата и реакции на них. |
|[Отправка сообщения в чате](../api/chat-post-messages.md) | [chatMessage](chatmessage.md)| Отправка сообщения чата в существующей беседе 1:1 или групповом чате.|
|[Обновление сообщения в чате](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление **свойства policyViolation** сообщения чата.|
|**Содержимое с хост-контентом**| | |
|[Список всего содержимого, на которое было организовано](../api/chatmessage-list-hostedcontents.md) | [коллекция chatMessageHostedContent](../resources/chatmessagehostedcontent.md)| Получите все содержимое, связанное с сообщением.|
|[Получить контент с хост-контентом](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | Получите у себя содержимое (и его bytes) для сообщения.|


## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный id сообщения.|
|replyToId| string | Только для чтения. Id родительского сообщения чата или корневого сообщения чата потока. (Применяется только к чатам в каналах, а не к чатам.) |
|from|[identitySet](identityset.md)| Только для чтения. Сведения о отправителье сообщения чата.|
|etag| string | Только для чтения. Номер версии сообщения чата. |
|messageType|Строка|Тип сообщения чата. Возможное значение: `message` .|
|createdDateTime|dateTimeOffset|Время создания сообщения чата.|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Timestamp, когда сообщение чата создается (начальный параметр) или изменено, в том числе при добавлении или удалении реакции. |
|lastEditedDateTime|dateTimeOffset|Только для чтения. Timestamp, когда были сделаны изменения в сообщении чата. Вызывает флаг "Отредактирован" Teams пользовательского интерфейса. Если изменение не выполнено, значение `null` .|
|deletedDateTime|dateTimeOffset|Только для чтения. Timestamp, при котором сообщение чата было удалено, или null, если не удалено. |
|subject|string| Тема сообщения чата в plaintext.|
|body|[itemBody](itembody.md)|Представление plaintext/HTML контента сообщения чата. Представление определяется параметром contentType в тексте. Содержимое всегда находится в HTML, если в сообщении чата [содержится chatMessageMention.](chatmessagemention.md) |
|summary|string| Сводный текст сообщения чата, который можно использовать для push-уведомлений и сводных представлений или отпадения представлений. Применяется только к сообщениям чата, а не к чатам в чате. |
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Вложенные файлы. В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается. |
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностями, упомянутыми в сообщении чата. В настоящее время поддерживаются значения user, bot, team и channel.|
|importance|string | Важность сообщения чата. Допустимые значения: `normal`, `high`, `urgent`.|
|reactions| Коллекция [chatMessageReaction](chatmessagereaction.md) | Реакции на это сообщение чата (например, Like).|
|языковые стандарты|string|Локализовать сообщение чата, за набором клиентом. Всегда задавайте значение `en-us`.|
|policyViolation | [chatMessagePolicyViolation](chatmessagepolicyviolation.md) |Определяет свойства нарушения политики, установленные приложением для предотвращения потери данных (DLP).|
|chatId|Строка|Если сообщение было отправлено в чате, представляет собой удостоверение чата.|
|channelIdentity|[channelIdentity](channelidentity.md)|Если сообщение было отправлено в канале, представляет удостоверение канала.|
|webUrl|string|Только для чтения. Ссылка на сообщение в Microsoft Teams.|
## <a name="relationships"></a>Отношения

| Связь   | Тип    | Описание |
|:---------------|:--------|:----------|
|ответы|[chatMessage](chatmessage.md)| Ответы на указанное сообщение. |
|hostedContents|[chatMessageHostedContent](chatmessagehostedcontent.md)| Содержимое в сообщении, которое Microsoft Teams - например, изображения, фрагменты кода и т. д. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "replyToId",
    "lastEditedDateTime",
    "deletedDateTime",
    "subject",
    "summary",
    "attachments",
    "mentions",
    "reactions",
    "policyViolation",
    "chatId",
    "channelIdentity"
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
  "lastEditedDateTime": "string (timestamp)",
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
  "webUrl": "string"
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
