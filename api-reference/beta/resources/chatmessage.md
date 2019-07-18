---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 99e69bd51a661b67fd4cb325fffe80db91214714
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778672"
---
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md).
Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление сообщений в канале](../api/channel-list-messages.md) | Коллекция [chatMessage](chatmessage.md) | Список всех корневых сообщений в канале.|
|[Получение сообщения в канале](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | Получение одного корневого сообщения из канала.|
|[Перечисление ответов на сообщение](../api/channel-list-messagereplies.md) | Коллекция [chatMessage](chatmessage.md)| Список всех ответов на сообщение в канале.|
|[Получение ответа на сообщение](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| Получение одного ответа на сообщение в канале.|
|[Создание chatMessage в канале](../api/channel-post-messages.md) | [chatMessage](chatmessage.md)| Создание сообщения верхнего уровня в канале.|
|[Ответ на сообщение в канале](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| Ответ на существующее сообщение в канале.|
|[Список сообщений в чате](../api/chatmessage-list.md)  | [chatMessage](../resources/chatmessage.md) | Перечисление сообщений в сообщениях в формате 1:1 или Group Chat. |
|[Получение сообщения в чате](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Получение одного сообщения в чате. |
|[Перечисление всех размещенных изображений](../api/chatmessagehostedimage-list-hostedimages.md) | Коллекция [хостедимаже](../resources/chatmessagehostedimage.md)| Получение всех размещенных изображений в сообщении.|
|[Получение размещенного изображения](../api/chatmessagehostedimage-get.md) | [Хостедимаже](../resources/chatmessagehostedimage.md) | Получение размещенного изображения из сообщения.|
|[Получение байтов размещенного изображения](../api/chatmessagehostedimage-getbytes.md) | данные двоичных изображений | Получение двоичных данных изображения на размещенном изображении из сообщения.|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|replyToId| string | Только для чтения. Идентификатор родительского или корневого сообщения беседы. (Применимо только к сообщениям в каналах, но не в чате) |
|from|[identitySet](identityset.md)| Только для чтения. Подробные сведения об отправителе сообщения.|
|etag| string | Только для чтения. Номер версии сообщения. |
|messageType|Чатмессажетипе|Тип сообщения. Возможные значения: `message`.|
|createdDateTime|dateTimeOffset|Только для чтения. Метка времени создания сообщения.|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Метка времени создания или изменения сообщения, включая время ответа (если это корневое сообщение в канале), а также добавление или удаление реакции. |
|deletedDateTime|dateTimeOffset|Только для чтения. Метка времени, в которое сообщение было удалено, или значение null, если сообщение не было удалено. |
|subject|string| Тема сообщения в формате обычного текста.|
|body|[itemBody](itembody.md)|Представление содержимого сообщения в формате Plaintext/HTML. Представление определяется параметром contentType в тексте. Содержимое всегда имеет формат HTML, если сообщение содержит [chatMessageMention](chatmessagemention.md). |
|summary|string| Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений. Относится только к сообщениям каналов, не к сообщениям чата. |
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Вложенные файлы. В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается. |
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностей, упомянутых в сообщении. В настоящее время поддерживаются значения user, bot, team и channel.|
|importance| Чатмессажеимпортанце | Важность сообщения. Допустимые значения: `normal`, `high`, `urgent`.|
|reactions| Коллекция [chatMessageReaction](chatmessagereaction.md) | Реакции на сообщение (например, "Нравится").|
|языковые стандарты|string|Язык сообщения, установленный клиентом.|

## <a name="json-representation"></a>Представление в формате JSON

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
