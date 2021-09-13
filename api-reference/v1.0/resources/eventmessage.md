---
title: Тип ресурса eventMessage
description: Сообщение, которое представляет собой приглашение на собрание, уведомление об отмене или ответ (принятие, предварительное принятие или отклонение).
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9a216718df8bb6245fb0138865f996de05809632
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067418"
---
# <a name="eventmessage-resource-type"></a>Тип ресурса eventMessage

Пространство имен: microsoft.graph

Сообщение, которое представляет собой приглашение на собрание, уведомление об отмене или ответ (принятие, предварительное принятие или отклонение).

Объект **eventMessage** является производным от объекта [message](message.md). **eventMessage** — это базовый тип [для eventMessageRequest](eventmessagerequest.md) и [eventMessageResponse.](eventmessageresponse.md) Свойство **meetingMessageType** определяет тип сообщения о событии.

Когда организатор или приложение отправляет запрос на собрание, запрос собрания поступает в почтовый ящик приглашенного в качестве экземпляра **eventMessage** с **meetingMessageType** **meetingRequest**. Кроме того, Outlook автоматически создает экземпляр  события в календаре приглашенных, а свойство **showAs** в качестве **предварительного**. 

Чтобы получить свойства связанного события в почтовом ящике приглашенного,  приложение может использовать свойство навигации событий **eventMessage,** как показано в этом примере сообщения [событий.](../api/eventmessage-get.md#example-2) Приложение также может реагировать на событие от имени приглашенных программным [](../api/event-tentativelyaccept.md)путем, принимая, [](../api/event-decline.md) предварительно принимая или уменьшая событие. [](../api/event-accept.md)

Помимо запроса на собрание, экземпляр **eventMessage** можно найти в почтовом ящике приглашенного в результате отмены собрания организатором события или в почтовом ящике организатора в результате ответа приглашенного на запрос собрания. Приложение может предпринимать с сообщениями о событиях те же действия, что и с обычными сообщения (с небольшими отличиями).
## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение объекта eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Считывание свойств и отношений объекта eventMessage.|
|[Обновление](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Обновление объекта eventMessage. |
|[удаление](../api/message-delete.md); | Нет |Удаление объекта eventMessage. |
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
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция [openTypeExtension](opentypeextension.md)| Получение объекта или объектов открытого расширения, которые определяются по имени или полному имени.|
|**Расширенные свойства**| | |
|[Создание однозначного расширенного свойства](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[eventMessage](eventmessage.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем экземпляре eventMessage.   |
|[Получение eventMessage с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Получение экземпляров eventMessage, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [eventMessage](eventmessage.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре eventMessage.  |
|[Получение eventMessage с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Получение eventMessage, которое содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bccRecipients|Коллекция [recipient](recipient.md)|Получатели скрытой копии сообщения.|
|body|[itemBody](itembody.md)|Текст сообщения. В формате HTML или текстовом формате.|
|bodyPreview|String|Первые 255 символов в тексте сообщения. В текстовом формате.|
|categories|Коллекция String|Категории, сопоставленные с сообщением.|
|ccRecipients|Коллекция [recipient](recipient.md)|Получатели копии сообщения.|
|changeKey|String|Версия сообщения.|
|conversationId|String|Идентификатор беседы, к которой принадлежит электронное сообщение.|
|conversationIndex|Edm.Binary|Указывает место сообщения в беседе.|
|createdDateTime|DateTimeOffset|Дата и время создания сообщения.|
|flag|[followupFlag](followupflag.md)|Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения сообщения.|
|from|[recipient](recipient.md)|Владелец почтового ящика, из которого отправлено сообщение. В большинстве случаев это значение совпадает со свойством **sender**, кроме сценариев предоставления общего доступа или делегирования. Значение должно соответствовать фактически используемому почтовому ящику. Дополнительные сведения о [задании свойств from и sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) сообщения.|
|hasAttachments|Boolean|Указывает на наличие вложений в сообщении.|
|id|String|Уникальный идентификатор для сообщения события (обратите внимание, что это значение может измениться при перемещении или изменении сообщения)|
|importance|String| Важность сообщения: `low`, `normal`, `high`.|
|inferenceClassification|String| Возможные значения: `focused` , `other` .|
|internetMessageHeaders | Коллекция [internetMessageHeader](internetmessageheader.md) | Коллекция заголовков сообщений, установленных по [RFC 5322](https://www.ietf.org/rfc/rfc5322.txt), которые содержат информацию о маршруте прохождения сообщения. Только для чтения.|
|internetMessageId |String |Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). |
|isDelegated|Boolean|True, если этот запрос собрания доступен делегату, ложный в противном случае. Значение по умолчанию: false.|
|isDeliveryReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|isDraft|Логическое|Указывает, является ли сообщение черновиком. Сообщение считается черновиком, если оно еще не отправлено.|
|isRead|Boolean|Указывает, прочитано ли сообщение.|
|isReadReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сообщения.|
|meetingMessageType|meetingMessageType| Тип сообщения о событии: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTenativelyAccepted`, `meetingDeclined`.|
|parentFolderId|String|Уникальный идентификатор родительского ресурса mailFolder для сообщения.|
|receivedDateTime|DateTimeOffset|Дата и время получения сообщения.|
|replyTo|Коллекция [recipient](recipient.md)|Электронные адреса, которые необходимо использовать при ответе.|
|sender|[recipient](recipient.md)|Учетная запись, которая фактически используется для создания сообщения. В большинстве случаев это значение совпадает со значением свойства **from**. Этому свойству можно присвоить другое значение при отправке сообщения из [общего почтового ящика](/exchange/collaboration/shared-mailboxes/shared-mailboxes), [для общего календаря или в качестве делегата](/graph/outlook-share-delegate-calendar.md). В любом случае значение должно соответствовать фактически используемому почтовому ящику. Дополнительные сведения о [задании свойств from и sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) сообщения.|
|sentDateTime|DateTimeOffset|Дата и время отправки сообщения.|
|subject|String|Тема сообщения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели сообщения, указанные в поле "Кому".|
|uniqueBody|[itemBody](itembody.md)|Часть текста сообщения, которая является уникальной для текущего сообщения.|
|webLink|String|URL-адрес для открытия сообщения в Outlook в Интернете.<br><br>Чтобы изменить способ отображения сообщения, можно добавить аргумент ispopout в конце URL-адреса. Если аргумент ispopout отсутствует или для него задано значение 1, то сообщение откроется во всплывающем окне. Если для аргумента ispopout задано значение 0, то в браузере сообщение будет отображаться в области просмотра Outlook в Интернете.<br><br>Сообщение откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br><br>Доступ к этому URL-адресу невозможно получить из объекта iFrame.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md) | Только для чтения. Допускается значение null.|
|event|[event](event.md)| Событие, связанное с сообщением о событии. Для участников или ресурсов помещений предполагается, что помощник по ведению календаря настроен для автоматического обновления события в календаре, если поступают сообщения с приглашением на собрание. Свойство навигации.  Только для чтения.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для сообщения о событии. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для eventMessage. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для eventMessage. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.  

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.message",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.message",
  "@odata.type": "microsoft.graph.eventMessage",
  "@odata.annotations": [
    {
      "property": "event",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
  "conversationIndex": "String (binary)",
  "createdDateTime": "DateTimeOffset",
  "event": { "@odata.type": "microsoft.graph.event" },
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isDelegated": true,
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "DateTimeOffset",
  "meetingMessageType": "String",
  "parentFolderId": "string",
  "receivedDateTime": "DateTimeOffset",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "DateTimeOffset",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

