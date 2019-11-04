---
title: Тип ресурса eventMessageRequest
description: Сообщение, представляющее приглашение на собрание.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f7cf6d2a0c040053d03e74de1991b7db675ff977
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939413"
---
# <a name="eventmessagerequest-resource-type"></a>Тип ресурса eventMessageRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сообщение, представляющее приглашение на собрание в почтовом ящике приглашений.

Сущность **eventMessageRequest** является производной от [eventMessage](eventmessage.md).

Чтобы ответить на приглашение на собрание, сначала используйте свойство навигации **event** , чтобы получить доступ к соответствующему событию, как показано в этом [примере](../api/eventmessage-get.md#example-2). Затем [примите](../api/event-accept.md), [тентативелякцепт](../api/event-tentativelyaccept.md)или [отклоните](../api/event-decline.md) событие, связанное с **eventMessageRequest**.

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
    "mentions",
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
  "mentionsPreview": {"@odata.type": "microsoft.graph.mentionsPreview"},
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
|changeKey|Строка|Версия сообщения.|
|conversationId|Строка|Идентификатор беседы, к которой принадлежит электронное сообщение.|
|conversationIndex|Edm.Binary|Индекс беседы, к которой относится электронная почта.|
|createdDateTime|DateTimeOffset|Дата и время создания сообщения.|
|endDateTime|[DateTimeTimeZone](datetimetimezone.md)|Время окончания запрошенного собрания.|
|from|[recipient](recipient.md)|Владелец почтового ящика и отправитель сообщения.|
|hasAttachments|Boolean|Указывает на наличие вложений в сообщении.|
|id|Строка|Только для чтения.|
|importance|String| Важность сообщения: `Low`, `Normal`, `High`.|
|inferenceClassification|Строка| Возможные значения: `Focused`, `Other`.|
|Isdelegated для|Логический|Значение true, если ответ на приглашение на собрание доступен представителю, в противном случае — значение false. Значение по умолчанию — false.|
|isDeliveryReceiptRequested|Логический|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|isDraft|Логическое|Указывает, является ли сообщение черновиком. Сообщение считается черновиком, если оно еще не отправлено.|
|isOutOfDate|Логический|Указывает, было ли это приглашение на собрание отменено в последний запрос.|
|isRead|Логический|Указывает, прочитано ли сообщение.|
|isReadReceiptRequested|Логический|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сообщения.|
|location|[Location](location.md)|Расположение запрошенного собрания.|
|meetingMessageType|String| Тип сообщения о событии: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|mentionsPreview|[mentionsPreview](mentionspreview.md)|Сведения об упоминаниях в сообщении. При обработке запроса `GET` /messages сервер устанавливает это свойство и включает его в отклик по умолчанию. Сервер возвращает значение null, если в сообщении нет упоминаний. Необязательное свойство. |
|parentFolderId|Строка|Уникальный идентификатор родительского ресурса mailFolder для сообщения.|
|превиаусенддатетиме|[DateTimeTimeZone](datetimetimezone.md)| Если в обновлении собрания изменяется время окончания собрания, это свойство указывает время окончания предыдущего собрания.|
|превиауслокатион|[Location](location.md)| Если в процессе обновления собрания изменяется место проведения собрания, это свойство указывает предыдущее место проведения собрания.|
|превиаусстартдатетиме|[DateTimeTimeZone](datetimetimezone.md)| Если при обновлении собрания изменяется время начала собрания, это свойство указывает время начала предыдущего собрания.|
|receivedDateTime|DateTimeOffset|Дата и время получения сообщения.|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|Шаблон повторения запрошенного собрания.|
|replyTo|Коллекция [recipient](recipient.md)|Электронные адреса, которые необходимо использовать при ответе.|
|responseRequested|Логический|Задайте значение true, если отправитель хочет отправить ответ на запрошенное собрание.|
|sender|[recipient](recipient.md)|Учетная запись, которая фактически используется для создания сообщения.|
|sentDateTime|DateTimeOffset|Дата и время отправки сообщения.|
|startDateTime|[DateTimeTimeZone](datetimetimezone.md)|Время начала запрошенного собрания.|
|subject|Строка|Тема сообщения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели сообщения, указанные в поле "Кому".|
|type|String|Тип запрошенного собрания `singleInstance`:, `occurence`, `exception`,. `seriesMaster`|
|uniqueBody|[itemBody](itembody.md)|Часть текста сообщения, которая является уникальной для текущего сообщения.|
|webLink|String|URL-адрес для открытия сообщения в Outlook Web App.<br><br>Чтобы изменить способ отображения сообщения, можно добавить аргумент ispopout в конце URL-адреса. Если аргумент ispopout отсутствует или для него задано значение 1, то сообщение откроется во всплывающем окне. Если для аргумента ispopout задано значение 0, то в браузере сообщение будет отображаться в области просмотра Outlook Web App.<br><br>Сообщение откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook Web App. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br><br>Доступ к этому URL-адресу можно получить из объекта iFrame.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md) |Коллекция вложений [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md)и [referenceAttachment](referenceattachment.md) для сообщения. Только для чтения. Допускается значение null.|
|event|[event](event.md)| Событие, связанное с сообщением о событии. Для участников или ресурсов помещений предполагается, что помощник по ведению календаря настроен для автоматического обновления события в календаре, если поступают сообщения с приглашением на собрание. Свойство навигации.  Только для чтения.|
|extensions|Коллекция [extension](extension.md)| Коллекция открытых расширений, определенных для сообщения о событии. Только для чтения. Допускается значение null.|
|mentions|Коллекция [mention](mention.md) | Коллекция упоминаний в сообщении, упорядоченных по свойству **createdDateTime** от новых к старым. По умолчанию запрос `GET` /messages не возвращает это свойство, если к свойству не применен параметр `$expand`.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для eventMessage. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для eventMessage. Только для чтения. Допускается значение null.|


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Считывание свойств и отношений объекта eventMessage.|
|[Обновление](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Обновление объекта eventMessage.|
|[Delete](../api/eventmessage-delete.md) | Нет. |Удаление объекта eventMessage.|
|[copy](../api/message-copy.md)|[message](message.md)|Копирование сообщения в папку.|
|[createForward](../api/message-createforward.md)|[message](message.md)|Создание черновика пересылаемого сообщения. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[createReply](../api/message-createreply.md)|[message](message.md)|Создание черновика ответного сообщения. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[createReplyAll](../api/message-createreplyall.md)|[message](message.md)|Создание черновика сообщения для ответа всем пользователям. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[forward](../api/message-forward.md)|Нет.|Пересылка сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[move](../api/message-move.md)|[message](message.md)|Перемещение сообщения в папку. При этом в целевой папке создается новая копия сообщения.|
|[reply](../api/message-reply.md)|Нет.|Ответ отправителю сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[replyAll](../api/message-replyall.md)|Нет.|Ответ всем получателям сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[send](../api/message-send.md)|Нет|Отправка ранее созданного черновика сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[unsubscribe](../api/message-unsubscribe.md)|Нет|Отправка сообщения, используя данные и адрес, указанные в это первой команде mailto заголовка List-Unsubscribe.|
|**Вложения**| | |
|[Список вложений](../api/eventmessage-list-attachments.md) |Коллекция [attachment](attachment.md) | Получение всех файлов, вложенных в сообщение о событии.|
|[Добавление вложения](../api/eventmessage-post-attachments.md) |[attachment](attachment.md)| Вложение в сообщение о событии нового файла путем публикации в коллекции вложений.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определенного по имени.|
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
