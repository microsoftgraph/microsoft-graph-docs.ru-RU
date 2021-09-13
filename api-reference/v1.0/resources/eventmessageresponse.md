---
title: тип ресурса eventMessageResponse
description: Сообщение, представляющие ответ на запрос собрания в почтовом ящике организатора собрания.
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1e07b7cd2271b47605311ce2d58202e844f4c0bc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067398"
---
# <a name="eventmessageresponse-resource-type"></a>тип ресурса eventMessageResponse

Пространство имен: microsoft.graph

Сообщение, представляющие ответ на запрос собрания в почтовом ящике организатора собрания.

Производный от [eventMessage](eventmessage.md). 

Организатор, который получает **eventMessageResponse** с набором **responseType** или , который включает предлагаемое `tentativelyAccepted` `declined` **свойствоNewTime,** может принять предложение. Для этого сначала используйте  свойство навигации событий **eventMessageResponse** для доступа к соответствующему событию, как показано в этом [примере.](../api/eventmessage-get.md#example-2) Затем [обновим](../api/event-update.md) связанное событие до предложенного времени.

Дополнительные сведения о том, как предложить время, а также как получить и принять новое предложение времени, см. в дополнительных сведениях о том, как предложить [новое время собраний.](/graph/outlook-calendar-meeting-proposals)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
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


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|bccRecipients|Коллекция [recipient](recipient.md)|Получатели скрытой копии сообщения.|
|body|[itemBody](itembody.md)|Текст сообщения. В формате HTML или текстовом формате.|
|bodyPreview|String|Первые 255 символов в тексте сообщения. В текстовом формате. |
|categories|Коллекция String|Категории, сопоставленные с сообщением.|
|ccRecipients|Коллекция [recipient](recipient.md)|Получатели копии сообщения.|
|changeKey|String|Версия сообщения.|
|conversationId|String|Идентификатор беседы, к которой принадлежит электронное сообщение.|
|conversationIndex|Edm.Binary|Индекс беседы, к которой принадлежит электронное сообщение.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|Конечное время запрашиваемого собрания.|
|flag|[followupFlag](followupflag.md)|Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения сообщения.|
|from|[recipient](recipient.md)|Владелец почтового ящика, из которого отправлено сообщение. В большинстве случаев это значение совпадает со свойством **sender**, кроме сценариев предоставления общего доступа или делегирования. Значение должно соответствовать фактически используемому почтовому ящику. Дополнительные сведения о [задании свойств from и sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) сообщения.|
|hasAttachments|Boolean|Указывает на наличие вложений в сообщении.|
|id|String| Уникальный идентификатор сообщения. [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] Только для чтения. |
|importance|String| Важность сообщения: `low`, `normal`, `high`.|
|inferenceClassification|String| Возможные значения: `focused`, `other`.|
|internetMessageHeaders | Коллекция [internetMessageHeader](internetmessageheader.md) | Коллекция заголовков сообщений, установленных по [RFC 5322](https://www.ietf.org/rfc/rfc5322.txt), которые содержат информацию о маршруте прохождения сообщения. Только для чтения.|
|internetMessageId |String |Идентификатор сообщения в формате, установленном документом [RFC5322](https://www.ietf.org/rfc/rfc5322.txt). |
|isAllDay |Boolean|Указывает, длится ли событие весь день. Для настройки этого свойства необходимо также настроить **свойства startDateTime** и **endDateTime** события.|
|isDelegated|Boolean|True, если ответ запроса на собрание доступен делегату, ложный в противном случае. Значение по умолчанию: false.|
|isDeliveryReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|isDraft|Логическое|Указывает, является ли сообщение черновиком. Сообщение считается черновиком, если оно еще не отправлено.|
|isOutOfDate|Boolean|Указывает, был ли этот запрос собрания устарел по более недавнему запросу.|
|isRead|Boolean|Указывает, прочитано ли сообщение.|
|isReadReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|lastModifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|location|[location](location.md)|Расположение запрашиваемого собрания.|
|meetingMessageType|String| Тип сообщения о событии: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|parentFolderId|String|Уникальный идентификатор родительского ресурса mailFolder для сообщения.|
|proposedNewTime|[timeSlot](timeslot.md)|Альтернативные даты и времени, предлагаемые приглашенным для запроса на собрание, чтобы начать и закончить. Только для чтения. Не фильтруется.|
|receivedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Шаблон повторения запрашиваемого собрания.|
|replyTo|Коллекция [recipient](recipient.md)|Электронные адреса, которые необходимо использовать при ответе.|
|responseType|string| Указывает тип ответа на запрос собрания. Возможные значения: `tentativelyAccepted`, `accepted`, `declined`. Для типа eventMessageResponse `none` , и не `organizer` `notResponded` поддерживается. Только для чтения. Не фильтруется.|
|sender|[recipient](recipient.md)|Учетная запись, которая фактически используется для создания сообщения. В большинстве случаев это значение совпадает со значением свойства **from**. Этому свойству можно присвоить другое значение при отправке сообщения из [общего почтового ящика](/exchange/collaboration/shared-mailboxes/shared-mailboxes), [для общего календаря или в качестве делегата](/graph/outlook-share-delegate-calendar.md). В любом случае значение должно соответствовать фактически используемому почтовому ящику. Дополнительные сведения о [задании свойств from и sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) сообщения.|
|sentDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|Время начала запрашиваемого собрания.|
|subject|String|Тема сообщения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели сообщения, указанные в поле "Кому".|
|type|Строка|Тип запрашиваемого собрания: `singleInstance` `occurence` , , `exception` `seriesMaster` .|
|uniqueBody|[itemBody](itembody.md)|Часть текста сообщения, которая является уникальной для текущего сообщения.|
|webLink|String|URL-адрес для открытия сообщения в Outlook в Интернете.<br><br>Чтобы изменить способ отображения сообщения, можно добавить аргумент ispopout в конце URL-адреса. Если аргумент ispopout отсутствует или для него задано значение 1, то сообщение откроется во всплывающем окне. Если для аргумента ispopout задано значение 0, то в браузере сообщение будет отображаться в области просмотра Outlook в Интернете.<br><br>Сообщение откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br><br>Доступ к этому URL-адресу невозможно получить из объекта iFrame.|


## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|attachments|Коллекция [attachment](attachment.md) |Коллекция вложений [fileAttachment,](fileattachment.md) [itemAttachment](itemattachment.md)и [referenceAttachment](referenceattachment.md) для сообщения. Только для чтения. Допускается значение null.|
|event|[event](event.md)| Событие, связанное с сообщением о событии. Для участников или ресурсов помещений предполагается, что помощник по ведению календаря настроен для автоматического обновления события в календаре, если поступают сообщения с приглашением на собрание. Свойство навигации.  Только для чтения.|
|extensions|Коллекция [extension](extension.md)| Коллекция открытых расширений, определенных для сообщения о событии. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для eventMessage. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для eventMessage. Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.eventMessageResponse",
  "baseType": "microsoft.graph.eventMessage",
  "keyProperty": "id"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "String",
  "categories": ["String"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "String",
  "conversationId": "String",
  "conversationIndex": "String (binary)",
  "createdDateTime": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "String (identifier)",
  "importance": "string",
  "inferenceClassification": "string",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isAllDay": true,
  "isDelegated": true,
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "string",
  "parentFolderId": "String",
  "proposedNewTime": {"@odata.type": "microsoft.graph.timeSlot"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "responseType": "string",
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "String",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessageResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
