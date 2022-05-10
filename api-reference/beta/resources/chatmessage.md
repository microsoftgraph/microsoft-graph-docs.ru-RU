---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в сущности канала или чата. Сообщение чата может быть корневым сообщением чата или частью потока, определенного **свойством replyToId** в сообщении чата.
doc_type: resourcePageType
ms.localizationpriority: medium
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: cc1651a8ea1d9ae5ca7a6dca2d4544cc3b8c735b
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296544"
---
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md). Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.

> **Примечание**. Этот ресурс поддерживает подписку на изменения (создание, обновление и удаление) с помощью [уведомлений об изменениях](../resources/webhooks.md). Это позволяет вызывающим подписаться на изменения и получать их в режиме реального времени. Дополнительные сведения см. в разделе [Получение уведомлений о сообщениях](/graph/teams-changenotifications-chatMessage).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Сообщения в канале**| | |
|[Вывод списка сообщений в канале](../api/channel-list-messages.md) | Коллекция [chatMessage](chatmessage.md) | Список всех корневых сообщений в канале.|
|[Получение разностных сообщений в канале](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Получение добавочных сообщений в канале. |
|[Создание подписки для новых сообщений канала](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Прослушивайте новые, измененные и удаленные сообщения и реакции на них. |
|[Получение сообщения в канале](../api/chatmessage-get.md) | [chatMessage](chatmessage.md) | Получение одного корневого сообщения в канале.|
|[Отправка сообщения в канале](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| Создайте новое корневое сообщение в канале.|
|[Обновление сообщения в канале](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление свойства **policyViolation** сообщения чата.|
|**Ответы на сообщения канала**| | |
|[Перечисление ответов на сообщение](../api/chatmessage-list-replies.md) | Коллекция [chatMessage](chatmessage.md)| Список всех ответов на сообщение чата в канале.|
|[Получение ответного сообщения в канале](../api/chatmessage-get.md) | [chatMessage](chatmessage.md) | Получение одного ответного сообщения в канале.|
|[Ответ на сообщение в канале](../api/chatmessage-post-replies.md) | [chatMessage](chatmessage.md)| Ответ на существующее сообщение чата в канале.|
|[Обновление ответного сообщения](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление свойства **policyViolation** сообщения чата.|
|**Сообщения чата**| | |
|[Вывод списка сообщений в чате](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Вывод списка сообщений чата в чате. |
|[Получение сообщения в чате](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Получение одного сообщения чата в чате. |
|[Получение сообщений во всех чатах для пользователя](../api/chats-getallmessages.md)| [коллекция чатов](chat.md)| Получение сообщений из всех чатов, в которых пользователь является участником, включая чаты 1:1, групповые чаты и чаты собраний. |
|[Получение всех сообщений в канале](../api/channel-getallmessages.md)|Коллекция [channel](channel.md) | Получайте все сообщения каналов, в которые входит пользователь. |
|[Создание подписки для новых сообщений чата](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Прослушивайте новые, измененные и удаленные сообщения чата и реакции на них. |
|[Отправка сообщения в чате](../api/chat-post-messages.md) | [chatMessage](chatmessage.md)| Отправка сообщения чата в существующей беседе 1:1 или групповой беседе.|
|[Обновление сообщения в чате](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление свойства **policyViolation** сообщения чата.|
|**Размещенное содержимое**| | |
|[Вывод списка всего размещенного содержимого](../api/chatmessage-list-hostedcontents.md) | [Коллекция chatMessageHostedContent](../resources/chatmessagehostedcontent.md)| Получение всего размещенного содержимого, связанного с сообщением.|
|[Получение размещенного содержимого](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | Получение размещенного содержимого (и его байтов) для сообщения.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Ссылки на вложенные объекты, такие как файлы, вкладки, собрания и т. д.|
|body|[itemBody](itembody.md)|Обычное текстовое или HTML-представление содержимого сообщения чата. Представление определяется параметром contentType в тексте. Содержимое всегда находится в ФОРМАТЕ HTML, если сообщение чата содержит [chatMessageMention](chatmessagemention.md). |
|channelIdentity|[channelIdentity](channelidentity.md)|Если сообщение было отправлено в канале, представляет удостоверение канала.|
|chatId|строка|Если сообщение было отправлено в **чате**, представляет удостоверение **чата**.|
|createdDateTime|dateTimeOffset|Метка времени создания сообщения чата.|
|deletedDateTime|dateTimeOffset|Только для чтения. Метка времени, в которой сообщение чата было удалено, или значение NULL, если оно не удалено. |
|etag| string | Только для чтения. Номер версии сообщения чата. |
|eventDetail|[eventMessageDetail](../resources/eventmessagedetail.md)|Только для чтения.  При наличии представляет сведения о событии, которое произошло в чате **, канале** или **команде**, например добавление новых участников. Для сообщений о событиях **свойству messageType** будет задано значение `systemEventMessage`.|
|from|[chatMessageFromIdentitySet](chatmessagefromidentityset.md)| Сведения об отправителях сообщения чата. Можно задать только во время [миграции](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|importance|строка | Важность сообщения чата. Допустимые значения: `normal`, `high`, `urgent`.|
|lastEditedDateTime|dateTimeOffset|Только для чтения. Метка времени при внесении изменений в сообщение чата. Активирует флаг "Изменено" в Teams пользовательского интерфейса. Если изменения не внесены, значение равно .`null`|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Метка времени при создании сообщения чата (начальном параметре) или изменении, в том числе при добавлении или удалении реакции. |
|языковые стандарты|string|Языковой стандарт сообщения чата, задаемого клиентом. Всегда задавайте значение `en-us`.|
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностей, упомянутых в сообщении чата. Поддерживаемые сущности: пользователь, бот, команда, канал и тег.|
|messageType|chatMessageType|Тип сообщения чата. Допустимые значения: `message`, `chatEvent`, `typing`, `unknownFutureValue`, `systemEventMessage`. Обратите внимание, что требуется использоваться заголовок запроса `Prefer: include-unknown-enum-members`, чтобы получить следующее значение в этом [расширяемом перечислении](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `systemEventMessage`.|
|onBehalfOf|[chatMessageFromIdentitySet](chatmessagefromidentityset.md)| Атрибут пользователя сообщения, когда [бот](/microsoftteams/platform/messaging-extensions/how-to/action-commands/respond-to-task-module-submit?tabs=dotnet%2Cdotnet-1#user-attribution-for-bots-messages) отправляет сообщение от имени пользователя.|
|policyViolation | [chatMessagePolicyViolation](chatmessagepolicyviolation.md) |Определяет свойства нарушения политики, заданные приложением защиты от потери данных (DLP).|
|reactions| Коллекция [chatMessageReaction](chatmessagereaction.md) | Реакции на это сообщение чата (например, Like).|
|replyToId| string | Только для чтения. Идентификатор родительского сообщения чата или сообщения корневого чата потока. (Применяется только к сообщениям чата в каналах, а не к чатам.) |
|subject|string| Тема сообщения чата в виде открытого текста.|
|summary|string| Сводный текст сообщения чата, который может использоваться для push-уведомлений и сводных представлений или резервных представлений. Применяется только к сообщениям чата канала, а не к чатам в чате. |
|webUrl|string|Только для чтения. Ссылка на сообщение в Microsoft Teams.|

## <a name="relationships"></a>Связи

| Связь   | Тип    | Описание |
|:---------------|:--------|:----------|
|Ответы|[chatMessage](chatmessage.md)| Отвечает за указанное сообщение. Поддерживает сообщения `$expand` канала. |
|hostedContents|[chatMessageHostedContent](chatmessagehostedcontent.md)| Содержимое в сообщении, размещенном Microsoft Teams, например изображения или фрагменты кода. |

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
