---
title: Тип ресурса eventMessageRequest
description: Сообщение, которое представляет приглашения на собрание.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5350b864ee38774f5b329110de6caf41f23dfe37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981100"
---
# <a name="eventmessagerequest-resource-type"></a>Тип ресурса eventMessageRequest

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сообщение, которое представляет приглашения на собрание.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "previousLocation",
    "previousStartDateTime",
    "previousEndDateTime"
  ],
  "@odata.type": "microsoft.graph.eventMessageRequest"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "microsoft.graph.meetingMessageType",
  "parentFolderId": "string",
  "previousEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "previousLocation": {"@odata.type": "microsoft.graph.location"},
  "previousStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bccRecipients|Коллекция [recipient](recipient.md)|Получатели скрытой копии сообщения.|
|body|[itemBody](itembody.md)|Текст сообщения.|
|bodyPreview|String|Первые 255 символов в тексте сообщения.|
|categories|Коллекция String|Категории, сопоставленные с сообщением.|
|ccRecipients|Коллекция [recipient](recipient.md)|Получатели копии сообщения.|
|changeKey|String|Версия сообщения.|
|conversationId|String|Идентификатор беседы, к которой принадлежит электронное сообщение.|
|createdDateTime|DateTimeOffset|Дата и время создания сообщения.|
|endDateTime|[DateTimeTimeZone](datetimetimezone.md)|Время окончания собрания запрошенного.|
|from|[recipient](recipient.md)|Владелец почтового ящика и отправитель сообщения.|
|hasAttachments|Boolean|Указывает на наличие вложений в сообщении.|
|id|Строка|Только для чтения.|
|importance|String| Важность сообщения: `Low`, `Normal`, `High`.|
|inferenceClassification|String| Возможные значения: `Focused`, `Other`.|
|isDeliveryReceiptRequested|Логический|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|isDraft|Boolean|Указывает, является ли сообщение черновиком. Сообщение считается черновиком, если оно еще не отправлено.|
|isOutOfDate|Логический|Указывает ли этот запрос на собрание было выполнено устаревших последних запроса.|
|isRead|Логический|Указывает, прочитано ли сообщение.|
|isReadReceiptRequested|Логический|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сообщения.|
|location|[Location](location.md)|Место собрания запрошенного.|
|meetingMessageType|String| Тип сообщения о событии: `None`, `MeetingRequest`, `MeetingCancelled`, `MeetingAccepted`, `MeetingTenativelyAccepted`, `MeetingDeclined`.|
|parentFolderId|String|Уникальный идентификатор родительского ресурса mailFolder для сообщения.|
|previousEndDateTime|[DateTimeTimeZone](datetimetimezone.md)|Время окончания предыдущей запрошенные собрания.|
|previousLocation|[Location](location.md)|Предыдущие место запрошенные собрания.|
|previousStartDateTime|[DateTimeTimeZone](datetimetimezone.md)|Время начала предыдущей запрошенные собрания.|
|receivedDateTime|DateTimeOffset|Дата и время получения сообщения.|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|Шаблон повторения запрошенные собрания.|
|replyTo|Коллекция [recipient](recipient.md)|Электронные адреса, которые необходимо использовать при ответе.|
|sender|[recipient](recipient.md)|Учетная запись, которая фактически используется для создания сообщения.|
|sentDateTime|DateTimeOffset|Дата и время отправки сообщения.|
|startDateTime|[DateTimeTimeZone](datetimetimezone.md)|Время начала запрошенные собрания.|
|subject|String|Тема сообщения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели сообщения, указанные в поле "Кому".|
|type|Строка|Тип запрошенного собрания: `singleInstance`, `occurence`, `exception`, `seriesMaster`.|
|uniqueBody|[itemBody](itembody.md)|Часть текста сообщения, которая является уникальной для текущего сообщения.|
|webLink|String|URL-адрес для открытия сообщения в Outlook Web App.<br><br>Чтобы изменить способ отображения сообщения, можно добавить аргумент ispopout в конце URL-адреса. Если аргумент ispopout отсутствует или для него задано значение 1, то сообщение откроется во всплывающем окне. Если для аргумента ispopout задано значение 0, то в браузере сообщение будет отображаться в области просмотра Outlook Web App.<br><br>Сообщение откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook Web App. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br><br>Доступ к этому URL-адресу можно получить из объекта iFrame.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция объектов [attachment](attachment.md)| Только для чтения. Допускается значение null.|
|event|[Event](event.md)| Событие, связанное с сообщением о событии. Для участников или ресурсов помещений предполагается, что помощник по ведению календаря настроен для автоматического обновления события в календаре, если поступают сообщения с приглашением на собрание. Свойство навигации.  Только для чтения.|
|extensions|Коллекция [extension](extension.md)| Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Считывание свойств и отношений объекта eventMessage.|
|[Создать подключение](../api/eventmessage-post-attachments.md) |[вложение](attachment.md);| Создание вложения путем записи в коллекцию вложений.|
|[Список вложений](../api/eventmessage-list-attachments.md) |Коллекция [Attachment](attachment.md)| Получение коллекции объектов Attachment.|
|[Обновление](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Обновление объекта eventMessage. |
|[Удаление](../api/eventmessage-delete.md) | Нет |Удаление объекта eventMessage. |
|[copy](../api/message-copy.md)|[Message](message.md)||
|[createForward](../api/message-createforward.md)|[Message](message.md)||
|[createReply](../api/message-createreply.md)|[Message](message.md)||
|[createReplyAll](../api/message-createreplyall.md)|[Message](message.md)||
|[forward](../api/message-forward.md)|Нет|Переадресует сообщение. Затем сообщение сохраняется в папке «Отправленные».|
|[move](../api/message-move.md)|[Message](message.md)|Перемещение сообщения в mailFolder.|
|[reply](../api/message-reply.md)|Нет|Ответы для отправителя сообщения. Затем сообщение сохраняется в папке «Отправленные».|
|[replyAll](../api/message-replyall.md)|Нет|Ответ всем получателям сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[send](../api/message-send.md)|Нет|Отправка ранее созданного черновика сообщения. После этого сообщение сохраняется в папке "Отправленные".|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
