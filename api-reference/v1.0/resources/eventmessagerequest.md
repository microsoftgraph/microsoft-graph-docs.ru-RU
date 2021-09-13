---
title: тип ресурса eventMessageRequest
description: Сообщение, представляю которое представляет запрос на собрание.
author: harini84
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1ef00be1e8f5a9881c62bbc11f79555334abfd04
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067411"
---
# <a name="eventmessagerequest-resource-type"></a>тип ресурса eventMessageRequest

Пространство имен: microsoft.graph

Сообщение, представляющие запрос на собрание в почтовом ящике приглашенного.

Объект **eventMessageRequest** происходит из [eventMessage.](eventmessage.md)

Чтобы ответить на запрос собрания, сначала используйте свойство **навигации** событий для доступа к соответствующему событию, как показано в этом [примере.](../api/eventmessage-get.md#example-2) Затем [примите](../api/event-accept.md), [предварительноAccept](../api/event-tentativelyaccept.md), или [отклонки,](../api/event-decline.md) что событие, связанное с **eventMessageRequest**.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.eventMessage",
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
  "allowNewTimeProposals": "Boolean",
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "conversationIndex": "String (binary)",
  "createdDateTime": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "isDelegated": true,
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
  "responseRequested": "Boolean",
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
|allowNewTimeProposals| Boolean | Значение `True`, если организатор собрания разрешает приглашенным предлагать новое время при ответе, в противном случае — `false`. Необязательный параметр. Значение по умолчанию: `true`. |
|bccRecipients|Коллекция [recipient](recipient.md)|Получатели скрытой копии сообщения.|
|body|[itemBody](itembody.md)|Текст сообщения.|
|bodyPreview|String|Первые 255 символов в тексте сообщения.|
|categories|Коллекция String|Категории, сопоставленные с сообщением.|
|ccRecipients|Коллекция [recipient](recipient.md)|Получатели копии сообщения.|
|changeKey|String|Версия сообщения.|
|conversationId|String|Идентификатор беседы, к которой принадлежит электронное сообщение.|
|conversationIndex|Edm.Binary|Индекс беседы, к которой принадлежит электронная почта.|
|createdDateTime|DateTimeOffset|Дата и время создания сообщения.|
|endDateTime|[DateTimeTimeZone](datetimetimezone.md)|Конечное время запрашиваемого собрания.|
|from|[recipient](recipient.md)|Владелец почтового ящика, из которого отправлено сообщение. В большинстве случаев это значение совпадает со свойством **sender**, кроме сценариев предоставления общего доступа или делегирования. Значение должно соответствовать фактически используемому почтовому ящику. Дополнительные сведения о [задании свойств from и sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) сообщения.|
|hasAttachments|Boolean|Указывает на наличие вложений в сообщении.|
|id|String|Только для чтения.|
|importance|String| Важность сообщения: `Low`, `Normal`, `High`.|
|inferenceClassification|String| Возможные значения: `Focused`, `Other`.|
|isDelegated|Boolean|True, если ответ запроса на собрание доступен делегату, ложный в противном случае. Значение по умолчанию: false.|
|isDeliveryReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|isDraft|Логическое|Указывает, является ли сообщение черновиком. Сообщение считается черновиком, если оно еще не отправлено.|
|isOutOfDate|Логический|Указывает, был ли этот запрос собрания устарел по более недавнему запросу.|
|isRead|Boolean|Указывает, прочитано ли сообщение.|
|isReadReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сообщения.|
|location|[Location](location.md)|Расположение запрашиваемого собрания.|
|meetingMessageType|String| Тип сообщения о событии: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|parentFolderId|String|Уникальный идентификатор родительского ресурса mailFolder для сообщения.|
|previousEndDateTime|[DateTimeTimeZone](datetimetimezone.md)| Если обновление собрания изменяет время окончания собрания, это свойство указывает предыдущее время окончания собрания.|
|previousLocation|[Location](location.md)| Если обновление собрания изменяет расположение собрания, это свойство указывает предыдущее расположение собрания.|
|previousStartDateTime|[DateTimeTimeZone](datetimetimezone.md)| Если обновление собрания изменяет время начала собрания, это свойство указывает предыдущее время начала собрания.|
|receivedDateTime|DateTimeOffset|Дата и время получения сообщения.|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|Шаблон повторения запрашиваемого собрания.|
|replyTo|Коллекция [recipient](recipient.md)|Электронные адреса, которые необходимо использовать при ответе.|
|responseRequested|Логический|Установите для true, если отправитель хотел бы, чтобы приглашенный отправил ответ на запрашиваемую встречу.|
|sender|[recipient](recipient.md)|Учетная запись, которая фактически используется для создания сообщения. В большинстве случаев это значение совпадает со значением свойства **from**. Этому свойству можно присвоить другое значение при отправке сообщения из [общего почтового ящика](/exchange/collaboration/shared-mailboxes/shared-mailboxes), [для общего календаря или в качестве делегата](/graph/outlook-share-delegate-calendar.md). В любом случае значение должно соответствовать фактически используемому почтовому ящику. Дополнительные сведения о [задании свойств from и sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) сообщения.|
|sentDateTime|DateTimeOffset|Дата и время отправки сообщения.|
|startDateTime|[DateTimeTimeZone](datetimetimezone.md)|Время начала запрашиваемого собрания.|
|subject|String|Тема сообщения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели сообщения, указанные в поле "Кому".|
|type|Строка|Тип запрашиваемого собрания: `singleInstance` `occurence` , , `exception` `seriesMaster` .|
|uniqueBody|[itemBody](itembody.md)|Часть текста сообщения, которая является уникальной для текущего сообщения.|
|webLink|String|URL-адрес для открытия сообщения в Outlook в Интернете.<br><br>Чтобы изменить способ отображения сообщения, можно добавить аргумент ispopout в конце URL-адреса. Если аргумент ispopout отсутствует или для него задано значение 1, то сообщение откроется во всплывающем окне. Если для аргумента ispopout задано значение 0, то в браузере сообщение будет отображаться в области просмотра Outlook в Интернете.<br><br>Сообщение откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br><br>Доступ к этому URL-адресу невозможно получить из объекта iFrame.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md) |Коллекция вложений [fileAttachment,](fileattachment.md) [itemAttachment](itemattachment.md)и [referenceAttachment](referenceattachment.md) для сообщения. Только для чтения. Допускается значение null.|
|event|[event](event.md)| Событие, связанное с сообщением о событии. Для участников или ресурсов помещений предполагается, что помощник по ведению календаря настроен для автоматического обновления события в календаре, если поступают сообщения с приглашением на собрание. Свойство навигации.  Только для чтения.|
|extensions|Коллекция [extension](extension.md)| Коллекция открытых расширений, определенных для сообщения о событии. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для eventMessage. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для eventMessage. Только для чтения. Допускается значение null.|


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Считывание свойств и отношений объекта eventMessage.|
|[Обновление](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Обновление объекта eventMessage.|
|[удаление](../api/eventmessage-delete.md); | Нет |Удаление объекта eventMessage.|
|[copy](../api/message-copy.md)|[message](message.md)|Копирование сообщения в папку.|
|[createForward](../api/message-createforward.md)|[message](message.md)|Создание черновика пересылаемого сообщения. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[createReply](../api/message-createreply.md)|[message](message.md)|Создание черновика ответного сообщения. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[createReplyAll](../api/message-createreplyall.md)|[message](message.md)|Создание черновика сообщения для ответа всем пользователям. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[forward](../api/message-forward.md)|Нет|Пересылка сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[move](../api/message-move.md)|[message](message.md)|Перемещение сообщения в папку. При этом в целевой папке создается новая копия сообщения.|
|[reply](../api/message-reply.md)|Нет|Ответ отправителю сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[replyAll](../api/message-replyall.md)|Нет|Ответ всем получателям сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[send](../api/message-send.md)|Нет|Отправка ранее созданного черновика сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|**Вложения**| | |
|[Список вложений](../api/eventmessage-list-attachments.md) |Коллекция [attachment](attachment.md) | Получение всех файлов, вложенных в сообщение о событии.|
|[Добавление вложения](../api/eventmessage-post-attachments.md) |[attachment](attachment.md)| Вложение в сообщение о событии нового файла путем публикации в коллекции вложений.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получите открытое расширение, идентифицированное по имени.|
|**Расширенные свойства**| | |
|[Создание однозначного расширенного свойства](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[eventMessage](eventmessage.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем экземпляре eventMessage.   |
|[Получение eventMessage с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Получение экземпляров eventMessage, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [eventMessage](eventmessage.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре eventMessage.  |
|[Получение eventMessage с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Получение eventMessage, которое содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

