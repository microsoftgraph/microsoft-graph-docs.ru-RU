---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в канале или в объекте Chat. Сообщение чата может быть корневым сообщением чата или частью потока, определенного свойством **реплитоид** в сообщении чата.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: bfaee36a21ee1f44781ea8ae7fed84b205ac90b4
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000650"
---
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md). Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.

> **Note** : этот ресурс поддерживает подписку на изменения (создание, обновление и удаление) с помощью [уведомлений об изменениях](../resources/webhooks.md). Это позволяет звонящим подписываться и получать изменения в режиме реального времени. Дополнительные сведения см. в статье [Получение уведомлений для сообщений](/graph/teams-changenotifications-chatMessage).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|**Сообщения канала**| | |
|[Список chatMessage Channel](../api/channel-list-messages.md) | Коллекция [chatMessage](chatmessage.md) | Список всех корневых сообщений чата в канале.|
|[Получение chatMessages в разностном канале](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Получение добавочных сообщений чата в канале. |
|[Создание подписки для сообщений о новых каналах](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Прослушивать новые и измененные сообщения каналов и реакции на них. |
|[Получение chatMessage Channel](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | Получение одного из каналов сообщения с одним корневым сеансом.|
|[Создание chatMessage в канале или чате](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| Создайте новое сообщение разговора верхнего уровня в канале.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление свойства **полицивиолатион** сообщения чата.|
|**Ответы на сообщения канала**| | |
|[Перечисление ответов на chatMessage](../api/channel-list-messagereplies.md) | Коллекция [chatMessage](chatmessage.md)| Список всех ответов на сообщение чата в канале.|
|[Получение ответа на chatMessage](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| Получение одного ответа на сообщение чата в канале.|
|[Ответ на chatMessage в канале](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| Ответ на существующее сообщение чата в канале.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление свойства **полицивиолатион** сообщения чата.|
|**1:1 и сообщения группового чата**| | |
|[Получение chatMessage в чате](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Получение одного сообщения чата в чате. |
|[Перечисление chatMessages в чате](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | Перечисление сообщений чата в 1:1 или группе чата. |
|[Создание подписки для новых сообщений чата](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Прослушивание новых и измененных сообщений чата и реакции на них. |
|[Создание chatMessage в чате](../api/chat-post-message.md) | [chatMessage](chatmessage.md)| Отправка сообщения чата в существующей беседе 1:1 или группе чата.|
|[Обновление chatMessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| Обновление свойства **полицивиолатион** сообщения чата.|
|**Размещенный контент**| | |
|[Перечисление всех размещенных контента](../api/chatmessage-list-chatmessagehostedcontents.md) | Коллекция [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md)| Получение всего размещенного содержимого в сообщении чата.|
|[Получение размещенного контента](../api/chatmessagehostedcontent-get.md) | [чатмессажехостедконтент](../resources/chatmessagehostedcontent.md) | Получение размещенного контента из сообщения чата.|


## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|replyToId| string | Только для чтения. Идентификатор родительского сообщения чата или сообщения корневого сеанса беседы в цепочке. (Это относится только к сообщениям разговора в каналах, а не к разговорам.) |
|from|[identitySet](identityset.md)| Только для чтения. Сведения об отправителе сообщения чата.|
|etag| string | Только для чтения. Номер версии сообщения чата. |
|messageType|строка|Тип сообщения чата. Возможные значения: `message` .|
|createdDateTime|dateTimeOffset|Только для чтения. Метка времени создания сообщения чата.|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Временная метка при создании или изменении сообщения чата (Начальная настройка), включая добавление или удаление реакции. |
|ластедитеддатетиме|dateTimeOffset|Только для чтения. Временная метка при внесении изменений в сообщение чата. Запускает в пользовательском интерфейсе Teams флаг "отредактирован". Если не выполняется никаких изменений, значение — `null` .|
|deletedDateTime|dateTimeOffset|Только для чтения. Временная метка, в которой сообщение чата удалено, или значение null, если оно не удалено. |
|subject|string| Тема сообщения чата в виде открытого текста.|
|body|[itemBody](itembody.md)|Представление содержимого сообщения чата в формате обычного текста или в формате HTML. Представление определяется параметром contentType в тексте. Если сообщение чата содержит [чатмессажементион](chatmessagemention.md), содержимое всегда находится в формате HTML. |
|summary|string| Сводный текст сообщения чата, которое можно использовать для push-уведомлений и сводных представлений, а также для обратного просмотра. Применяется только к сообщениям разговора по каналу, а не к сообщениям в чате. |
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Вложенные файлы. В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается. |
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностей, упоминаемых в сообщении чата. В настоящее время поддерживаются значения user, bot, team и channel.|
|importance|строка | Важность сообщения чата. Допустимые значения: `normal`, `high`, `urgent`.|
|reactions| Коллекция [chatMessageReaction](./chatmessagereaction.md) | Реакции на это сообщение чата (например, например).|
|языковые стандарты|string|Язык сообщения чата, заданное клиентом.|
| полицивиолатион | [чатмессажеполицивиолатион](../resources/chatmessagepolicyviolation.md) |Определяет свойства нарушения политики, заданные с помощью приложения предотвращения потери данных (DLP).|

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
