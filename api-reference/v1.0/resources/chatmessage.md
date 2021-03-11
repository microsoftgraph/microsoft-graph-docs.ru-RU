---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение чата может быть корневым сообщением чата или частью потока, определяемого **свойством replyToId** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 8099efac4132a070bfcf8443ef290989305d6737
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626133"
---
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

Пространство имен: microsoft.graph

Представляет отдельное сообщение чата в [канале](./channel.md) или (в бета-версии) [чата.](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true) Сообщение чата может быть корневым сообщением чата или частью потока ответа, определяемого **свойством replyToId** в сообщении чата.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Сообщения канала**| | |
|[Список каналов chatMessage](../api/channel-list-messages.md) | Коллекция [chatMessage](chatmessage.md) | Список всех корневых сообщений чата в канале.|
|[Получить chatMessages в дельте канала](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Получите дополнительные сообщения чата в канале. |
|[Создание подписки для новых сообщений канала](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Слушайте новые и отредактированы сообщения канала и реакции на них. |
|[Get channel chatMessage](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | Получите одно корневое сообщение чата из канала.|
|[Создание объекта chatMessage в канале](../api/channel-post-message.md) | [chatMessage](../resources/chatmessage.md) | Отправка сообщения в канал. |
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление **свойства policyViolation** сообщения чата.|
|**Ответы на сообщения канала**| | |
|[Ответы списка на chatMessage](../api/channel-list-messagereplies.md) | Коллекция [chatMessage](chatmessage.md)| Список всех ответов на сообщение чата в канале.|
|[Получить ответ на chatMessage](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| Получите один ответ на сообщение чата в канале.|
|[Ответ на chatMessage в канале](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| Ответ на существующее сообщение чата в канале.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление **свойства policyViolation** сообщения чата.|
|**Содержимое с хост-контентом**| | |
|[Список всего содержимого, на которое было организовано](../api/chatmessage-list-chatmessagehostedcontents.md) | [коллекция chatMessageHostedContent](../resources/chatmessagehostedcontent.md)| Получите все содержимое в сообщении чата.|
|[Получить контент с хост-контентом](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | Получите у себя содержимое из сообщения чата.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный id сообщения.|
|replyToId| string | Только для чтения. Id родительского сообщения чата или корневого сообщения чата потока. (Только для сообщений чата в каналах, а не в чатах) |
|from|[identitySet](identityset.md)| Только для чтения. Сведения о отправителье сообщения чата.|
|etag| string | Только для чтения. Номер версии сообщения чата. |
|messageType|Строка|Тип сообщения чата. Возможные значения: `message` .|
|createdDateTime|dateTimeOffset|Только для чтения. Время создания сообщения чата.|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Timestamp when the chat message is created (initial setting) or edited, including when a reaction is added or removed. |
|lastEditedDateTime|dateTimeOffset|Только для чтения. Timestamp, когда были сделаны изменения в сообщении чата. Вызывает флаг "Отредактирован" в пользовательском интерфейсе Microsoft Teams. Если изменение не выполнено, значение `null` .|
|deletedDateTime|dateTimeOffset|Только для чтения. Timestamp, при котором сообщение чата было удалено, или null, если не удалено. |
|subject|string| Тема сообщения чата в plaintext.|
|body|[itemBody](itembody.md)|Представление plaintext/HTML контента сообщения чата. Представление определяется параметром contentType в тексте. Содержимое всегда находится в HTML, если в сообщении чата [содержится chatMessageMention.](chatmessagemention.md) |
|summary|string| Сводный текст сообщения чата, который можно использовать для push-уведомлений и сводных представлений или отпадения представлений. Применяется только к сообщениям чата, а не к чатам в чате. |
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Вложенные файлы. В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается. |
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностями, упомянутыми в сообщении чата. В настоящее время поддерживаются значения user, bot, team и channel.|
|importance| string | Важность сообщения чата. Допустимые значения: `normal`, `high`, `urgent`.|
| policyViolation | [chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md) |Определяет свойства нарушения политики, установленные приложением для предотвращения потери данных (DLP).|
|языковые стандарты|string|Локализовать сообщение чата, за набором клиентом.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "mentions",
    "subject",
    "summary",
    "policyViolation",
    "locale"
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
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
  "locale": "string"
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
