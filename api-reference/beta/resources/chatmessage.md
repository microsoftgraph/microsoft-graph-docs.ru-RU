---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 0639fd0b5317abd4814123b500ec0548f78d05ac
ms.sourcegitcommit: abca7fcefeaa74b50f4600b35d816b626ba08468
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2019
ms.locfileid: "34311163"
---
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельное сообщение чата в [канале](channel.md) или [чате](chat.md). Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление сообщений в канале](../api/channel-list-messages.md) | Коллекция [chatmessage](chatmessage.md) | Получение списка всех корневых сообщений в канале.|
|[Получение сообщения в канале](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | Получение одного корневого сообщения из канала.|
|[Перечисление ответов на сообщение](../api/channel-list-messagereplies.md) | Коллекция [chatmessage](chatmessage.md)| Получение списка всех ответов на сообщение в канале.|
|[Получение ответа на сообщение](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| Получение одного ответа на сообщение в канале.|
|[Отправка сообщения в канал](../api/channel-post-chatmessage.md) | [chatmessage](chatmessage.md)| Создание сообщения верхнего уровня в канале.|
|[Ответ на сообщение в канале](../api/channel-post-messagereply.md) | [chatmessage](chatmessage.md)| Ответ на существующее сообщение в канале.|
|[Список сообщений в чате](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Получение сообщений в индивидуальном или групповом чате. |
|[Получение сообщения в чате](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Получение одного сообщения в чате. |


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|replyToId| string | Идентификатор родительского или корневого сообщения беседы. (Применимо только к сообщениям в каналах, но не в чате) |
|from|[identitySet](identityset.md)| Только для чтения. Подробные сведения об отправителе сообщения.|
|etag| string | Номер версии сообщения. |
|messageType|String|Тип сообщения. В настоящее время поддерживаются следующие значения: message, chatEvent, Typing.|
|createdDateTime|dateTimeOffset|Только для чтения. Метка времени создания сообщения.|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Метка времени изменения или обновления сообщения.|
|deletedDateTime|dateTimeOffset|Только для чтения. Метка времени, в которое сообщение было удалено, или значение null, если сообщение не было удалено. |
|subject|string| Тема сообщения в формате обычного текста.|
|body|[itemBody](itembody.md)|Представление содержимого сообщения в формате Plaintext/HTML. Представление определяется параметром contentType в тексте. Содержимое всегда имеет формат HTML, если сообщение содержит [chatMessageMention](chatmessagemention.md). |
|summary|string| Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений. Относится только к сообщениям каналов, не к сообщениям чата. |
|attachments|Коллекция [chatMessageAttachment](chatmessageattachment.md) |Вложенные файлы. В настоящее время вложения доступны только для чтения. Отправка вложений не поддерживается. |
|mentions|Коллекция [chatMessageMention](chatmessagemention.md)| Список сущностей, упомянутых в сообщении. В настоящее время поддерживаются значения user, bot, team и channel.|
|importance| string | Важность сообщения: Normal, High.|
|reactions| Коллекция [chatMessageReaction](chatmessagereaction.md) | Реакции на сообщение (например, "Нравится").|
|языковые стандарты|string|Язык сообщения, установленный клиентом.|
|webUrl|string|Гиперссылка, ведущая к каналу в Microsoft Teams. Это URL-адрес, получаемый при щелчке правой кнопкой мыши по каналу в Microsoft Teams и выборе пункта "Получить ссылку на канал". Этот URL-адрес должен обрабатываться как непрозрачный BLOB-объект и не должен анализироваться. Только для чтения.|

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
