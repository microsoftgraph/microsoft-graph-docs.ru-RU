---
title: Тип ресурса chatMessage
description: Представляет отдельное сообщение чата в объекте channel или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.
localization_priority: Priority
ms.openlocfilehash: f61668d8c3892482043dd7531a6699974a964527
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458661"
---
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отдельное сообщение чата в объекте [channel](channel.md) или chat. Сообщение может быть корневым или частью беседы, определяемой свойством **replyToId** в сообщении.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление сообщений в канале](../api/channel-list-messages.md) | Коллекция [chatmessage](chatmessage.md) | Получение списка всех корневых сообщений в канале.|
|[Получение сообщения в канале](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | Получение одного корневого сообщения из канала.|
|[Перечисление ответов на сообщение](../api/channel-list-messagereplies.md) | Коллекция [chatmessage](chatmessage.md)| Получение списка всех ответов на сообщение в канале.|
|[Получение ответа на сообщение](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| Получение одного ответа на сообщение в канале.|
|[Отправка сообщения в канал](../api/channel-post-chatmessage.md) | [chatmessage](chatmessage.md)| Создание сообщения верхнего уровня в канале.|
|[Ответ на сообщение в канале](../api/channel-post-messagereply.md) | [chatmessage](chatmessage.md)| Ответ на существующее сообщение в канале.|


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|replyToId| string | Идентификатор родительского или корневого сообщения беседы |
|from|[identitySet](identityset.md)| Сведения об отправителе сообщения|
|etag| string | Номер версии сообщения |
|messageType|String|Тип сообщения. Поддерживаемые в настоящее время значения: message, chatEvent, Typing|
|createdDateTime|dateTimeOffset|Только для чтения. Метка времени создания сообщения|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Метка времени изменения или обновления сообщения|
|deleted|Boolean|Указывает, удалено ли сообщение с возможностью восстановления|
|deletedDateTime|dateTimeOffset|Только для чтения. Метка времени удаления сообщения |
|subject|string|Строка темы сообщения. Необязательное|
|body|[itemBody](itembody.md)|Представление содержимого сообщения в формате Plaintext/HTML. Возвращает неформатированный текст по умолчанию. Приложение может выбрать формат HTML в составе параметров запроса|
|summary|string|Сводный текст сообщения, который можно использовать для push-уведомлений и представлений сводки или резервных представлений|
|mentions|Коллекция [chatMessageMention](chatmention.md)| Список сущностей, упомянутых в сообщении. Поддерживаемые в настоящее время: user, bot, team, channel|
|importance| string | Важность сообщения: высокая, низкая|
|reactions| Коллекция [chatMessageReaction](chatreaction.md) | Реакции на сообщение (например, "Нравится")|
|locale|string|Язык сообщения, установленный клиентом|
|attachments|Коллекция [chatMessageAttachment](chatattachment.md) |Вложенные файлы|


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
  "isDeleted": "boolean",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
