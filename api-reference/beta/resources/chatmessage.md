---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте канала или чата. Сообщение чата может быть корневым сообщением чата или частью потока, определяемого **свойством replyToId** в сообщении чата.
doc_type: resourcePageType
ms.localizationpriority: medium
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: 8b449c28f8283096696a6d95704de46cadaa8cfb
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860938"
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
|[Получение сообщений во всех чатах для пользователя](../api/chats-getallmessages.md)| [коллекция чатов](chat.md)| Получите сообщения из всех чатов, в которых пользователь является участником, включая чаты 1:1, групповые чаты и чаты собраний. |
|[Получение всех сообщений в канале](../api/channel-getallmessages.md)|Коллекция [channel](channel.md) | Получайте все сообщения каналов, в которые входит пользователь. |
|[Создание подписки для новых сообщений чата](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Слушайте новые, измененные и удаленные сообщения чата и реакции на них. |
|[Отправка сообщения в чате](../api/chat-post-messages.md) | [chatMessage](chatmessage.md)| Отправка сообщения чата в существующей беседе 1:1 или групповом чате.|
|[Обновление сообщения в чате](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление **свойства policyViolation** сообщения чата.|
|**Содержимое с хост-контентом**| | |
|[Список всего содержимого, на которое было организовано](../api/chatmessage-list-hostedcontents.md) | [коллекция chatMessageHostedContent](../resources/chatmessagehostedcontent.md)| Получите все содержимое, связанное с сообщением.|
|[Получить контент с хост-контентом](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | Получите у себя содержимое (и его bytes) для сообщения.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Ссылки на присоединенные объекты, такие как файлы, вкладки, собрания и т.д.|
|body|[itemBody](itembody.md)|Представление plaintext/HTML контента сообщения чата. Представление определяется параметром contentType в тексте. Содержимое всегда находится в HTML, если в сообщении чата [содержится chatMessageMention.](chatmessagemention.md) |
|channelIdentity|[channelIdentity](channelidentity.md)|Если сообщение было отправлено в канале, представляет удостоверение канала.|
|chatId|string|Если сообщение было отправлено в **чате,** представляет собой удостоверение **чата**.|
|createdDateTime|dateTimeOffset|Время создания сообщения чата.|
|deletedDateTime|dateTimeOffset|Только для чтения. Timestamp, при котором сообщение чата было удалено, или null, если не удалено. |
|etag| string | Только для чтения. Номер версии сообщения чата. |
|eventDetail|[eventMessageDetail](../resources/eventmessagedetail.md)|Только для чтения.  При этом представлены сведения о событии, произошедшем в чате, канале **или** **команде,** например добавление новых участников. Для сообщений событий будет установлено свойство **messageType** `systemEventMessage` .|
|from|[chatMessageFromIdentitySet](chatmessagefromidentityset.md)| Сведения о отправителье сообщения чата. Можно установить только во время [миграции.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|importance|string | Важность сообщения чата. Допустимые значения: `normal`, `high`, `urgent`.|
|lastEditedDateTime|dateTimeOffset|Только для чтения. Timestamp, когда были сделаны изменения в сообщении чата. Вызывает флаг "Отредактирован" Teams пользовательского интерфейса. Если изменение не выполнено, значение `null` .|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Timestamp, когда сообщение чата создается (начальный параметр) или изменено, в том числе при добавлении или удалении реакции. |
|языковые стандарты|string|Локализовать сообщение чата, за набором клиентом. Всегда задавайте значение `en-us`.|
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностями, упомянутыми в сообщении чата. Поддерживаемые сущности: пользователь, бот, команда, канал и теги.|
|messageType|chatMessageType|Тип сообщения чата. Допустимые значения: `message`, `chatEvent`, `typing`, `unknownFutureValue`, `systemEventMessage`. Обратите внимание, что требуется использоваться заголовок запроса `Prefer: include-unknown-enum-members`, чтобы получить следующее значение в этом [расширяемом перечислении](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `systemEventMessage`.|
|onBehalfOf|[chatMessageFromIdentitySet](chatmessagefromidentityset.md)| Присвоение пользователем сообщения при [отправке](/microsoftteams/platform/messaging-extensions/how-to/action-commands/respond-to-task-module-submit?tabs=dotnet%2Cdotnet-1#user-attribution-for-bots-messages) ботом сообщения от имени пользователя.|
|policyViolation | [chatMessagePolicyViolation](chatmessagepolicyviolation.md) |Определяет свойства нарушения политики, установленные приложением для предотвращения потери данных (DLP).|
|reactions| Коллекция [chatMessageReaction](chatmessagereaction.md) | Реакции на это сообщение чата (например, Like).|
|replyToId| string | Только для чтения. ID родительского сообщения чата или корневого сообщения чата потока. (Применяется только к чатам в каналах, а не к чатам.) |
|subject|string| Тема сообщения чата в plaintext.|
|summary|string| Сводный текст сообщения чата, который можно использовать для push-уведомлений и сводных представлений или отпадения представлений. Применяется только к сообщениям чата, а не к чатам в чате. |
|webUrl|string|Только для чтения. Ссылка на сообщение в Microsoft Teams.|

## <a name="relationships"></a>Связи

| Связь   | Тип    | Описание |
|:---------------|:--------|:----------|
|ответы|[chatMessage](chatmessage.md)| Ответы на указанное сообщение. |
|hostedContents|[chatMessageHostedContent](chatmessagehostedcontent.md)| Содержимое в сообщении, которое Microsoft Teams - например, изображения или фрагменты кода. |

## <a name="json-representation"></a>Представление JSON

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
  "from": {"@odata.type": "microsoft.graph.chatMessageFromIdentitySet"},
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
  "onBehalfOf": {"@odata.type": "microsoft.graph.chatMessageFromIdentitySet"},
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
  "chatId": "string",
  "channelIdentity": {"@odata.type": "microsoft.graph.channelIdentity"},
  "webUrl": "string",
  "eventDetail": {
    "@odata.type": "microsoft.graph.eventMessageDetail"
  }
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
