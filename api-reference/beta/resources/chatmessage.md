---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение чата может быть корневым сообщением чата или частью потока, определенного свойством **реплитоид** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 5443f88005f46a07353d6d24ed07bea11df7b30b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507721"
---
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md). Сообщение чата может быть корневым сообщением чата или частью ответа, которое определяется свойством **реплитоид** в сообщении чата.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Сообщения канала**| | |
|[Список chatMessage Channel](../api/channel-list-messages.md) | Коллекция [chatMessage](chatmessage.md) | Список всех корневых сообщений чата в канале.|
|[Получение chatMessages в разностном канале](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Получение добавочных сообщений чата в канале. |
|[Создание подписки для сообщений о новых каналах](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Прослушивать новые и измененные сообщения каналов и реакции на них. |
|[Получение chatMessage Channel](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | Получение одного из каналов сообщения с одним корневым сеансом.|
|[Создание объекта chatMessage в канале](../api/channel-post-messages.md) | [chatMessage](chatmessage.md)| Создайте новое сообщение разговора верхнего уровня в канале.|
|**Ответы на сообщения канала**| | |
|[Перечисление ответов на chatMessage](../api/channel-list-messagereplies.md) | Коллекция [chatMessage](chatmessage.md)| Список всех ответов на сообщение чата в канале.|
|[Получение ответа на chatMessage](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| Получение одного ответа на сообщение чата в канале.|
|[Ответ на chatMessage в канале](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| Ответ на существующее сообщение чата в канале.|
|**1:1 и сообщения группового чата**| | |
|[Создание chatMessage в чате](../api/chat-post-messages.md) | [chatMessage](chatmessage.md)| Отправка сообщения чата в существующей беседе 1:1 или группе чата.|
|[Перечисление chatMessages в чате](../api/chatmessage-list.md)  | [chatMessage](../resources/chatmessage.md) | Перечисление сообщений чата в 1:1 или группе чата. |
|[Создание подписки для новых сообщений чата](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Прослушивание новых и измененных сообщений чата и реакции на них. |
|[Получение chatMessage в чате](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Получение одного сообщения чата в чате. |
|**Размещенный контент**| | |
|[Перечисление всех размещенных контента](../api/chatmessage-list-chatmessagehostedcontents.md) | Коллекция [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md)| Получение всего размещенного содержимого в сообщении чата.|
|[Получение размещенного контента](../api/chatmessagehostedcontent-get.md) | [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) | Получение размещенного контента из сообщения чата.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|replyToId| string | Только для чтения. Идентификатор родительского сообщения чата или сообщения корневого сеанса беседы в цепочке. (Применяется только к сообщениям чата в каналах без чатов) |
|from|[identitySet](identityset.md)| Только для чтения. Сведения об отправителе сообщения чата.|
|etag| string | Только для чтения. Номер версии сообщения чата. |
|messageType|чатмессажетипе|Тип сообщения чата. Возможные значения: `message`.|
|createdDateTime|dateTimeOffset|Только для чтения. Метка времени создания сообщения чата.|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Метка времени создания или изменения сообщения чата, в том числе когда выполняется ответ (если он является корневым сообщением в канале) или добавляется или удаляется реакция. |
|deletedDateTime|dateTimeOffset|Только для чтения. Временная метка, в которой сообщение чата удалено, или значение null, если оно не удалено. |
|subject|string| Тема сообщения чата в виде открытого текста.|
|body|[itemBody](itembody.md)|Представление содержимого сообщения чата в формате обычного текста или в формате HTML. Представление определяется параметром contentType в тексте. Если сообщение чата содержит [чатмессажементион](chatmessagemention.md), содержимое всегда находится в формате HTML. |
|summary|string| Сводный текст сообщения чата, которое можно использовать для push-уведомлений и сводных представлений, а также для обратного просмотра. Применяется только к сообщениям разговора по каналу, а не к сообщениям в чате. |
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Вложенные файлы. В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается. |
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностей, упоминаемых в сообщении чата. В настоящее время поддерживаются значения user, bot, team и channel.|
|importance| чатмессажеимпортанце | Важность сообщения чата. Допустимые значения: `normal`, `high`, `urgent`.|
|reactions| Коллекция [chatMessageReaction](chatmessagereaction.md) | Реакции на это сообщение чата (например, например).|
|языковые стандарты|string|Язык сообщения чата, заданное клиентом.|

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
  "policyViolation": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
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
