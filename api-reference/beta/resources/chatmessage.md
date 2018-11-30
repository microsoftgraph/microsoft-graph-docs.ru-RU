---
title: Тип ресурса chatMessage
description: Представляет сообщение адресу сущности канала или чата. Сообщение может быть корневой сообщение или частью поток, который определяется свойством **replyToId** в сообщении.
ms.openlocfilehash: 1fba27567d5a1c80a36a5758925ec427735504cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074938"
---
# <a name="chatmessage-resource-type"></a>Тип ресурса chatMessage

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет сообщение адресу сущности [канала](channel.md) или чата. Сообщение может быть корневой сообщение или частью поток, который определяется свойством **replyToId** в сообщении.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список сообщения](../api/channel-list-messages.md) | [chatmessage](chatmessage.md) коллекции | Получение списка всех сообщений корневой в канал.|
|[Сообщение канала Get](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | Сообщение один корневой из канала.|
|[Список ответов на сообщение](../api/channel-list-messagereplies.md) | [chatmessage](chatmessage.md) коллекции| Получение списка всех ответов на сообщение в канала.|
|[Получить ответ на сообщение](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| Получите один ответ на сообщение в канале.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Только для чтения. Уникальный идентификатор сообщения.|
|replyToId| string | Идентификатор сообщения message/root родительского потока |
|from|[identitySet](identityset.md)| Сведения о отправитель сообщения|
|etag| string | Номер версии сообщения |
|messageType|String|Поддерживаемый тип сообщения текущего значения: сообщения, chatEvent, набор|
|createdDateTime|dateTimeOffset|Только для чтения. Метка времени создания сообщения|
|lastModifiedDateTime|dateTimeOffset|Только для чтения. Когда сообщение было изменяется обновлено отметки времени|
|isDeleted|boolean|Представляет Мягкая удаления сообщения|
|deletedDateTime|dateTimeOffset|Только для чтения. Метка времени, в котором оно было удалено |
|subject|строка|Строка темы сообщения. Необязательный|
|body|[itemBody](itembody.md)|Представление содержимое сообщения в обычный текст или HTML. Возвращает обычный текст по умолчанию, приложение может выбрать HTML в составе параметров запроса|
|Сводка|string|Сводки текста сообщения, которое может использоваться для push-уведомлений и представлений сводок или попадающих обратная представлений|
|упоминания|[chatMessageMention](chatmention.md) коллекции| Список сущностей, упомянутые в сообщении. В настоящее время поддерживает пользователя, программа-робот, группы, канала|
|importance| string | Важность сообщения: обычный, высокая|
|реакции| [chatMessageReaction](chatreaction.md) коллекции | Реакции для данного сообщения (например, например)|
|locale|string|Языковой стандарт сообщения, заданный клиентом|
|attachments|[chatMessageAttachment](chatattachment.md) коллекции |Вложенные файлы|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isDeleted",
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
<!-- {
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
