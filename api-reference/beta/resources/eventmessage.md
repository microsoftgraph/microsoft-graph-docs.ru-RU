---
title: Тип ресурса eventMessage
description: 'Сообщение, которое представляет собой приглашение на собрание, уведомление об отмене или ответ (принятие, предварительное принятие или отклонение). '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 926a9adc1a66ca912aff9a5ccea8db189eb4dae1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643421"
---
# <a name="eventmessage-resource-type"></a>Тип ресурса eventMessage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сообщение, которое представляет собой приглашение на собрание, уведомление об отмене или ответ (принятие, предварительное принятие или отклонение). 

Сущность **eventMessage** является производным от [сообщения](message.md), и [eventMessageRequest](eventmessagerequest.md) является производным от **eventMessage** и представляет приглашения на собрание. Свойство **meetingMessageType** определяет тип сообщения о событии.

Когда организатор или приложение отправляет приглашение на собрание, оно попадает во входящие участника в виде экземпляра **eventMessage** со свойством **meetingMessageType** **meetingRequest**. Кроме того, Outlook автоматически создает в календаре участника экземпляр **event** со свойством **showAs** **tentative**. 

Чтобы получить свойства связанного события в почтовом ящике участника, приложение может использовать свойство навигации объекта **eventMessage** **event**, как показано в [этом примере](../api/eventmessage-get.md#request-2). Приложения можно также отвечать на событие от имени участника программным способом, [Принятие](../api/event-accept.md), [под вопросом принятия](../api/event-tentativelyaccept.md)или [отклонения приглашения](../api/event-decline.md) события.

Помимо приглашения на собрание экземпляр **eventMessage** можно найти в папке "Входящие" участника в результате инициатора события отмены собрания или в папку "Входящие" организатора, из-за участником ответ на запрос на собрание. Приложение может предпринимать с сообщениями о событиях те же действия, что и с обычными сообщения (с небольшими отличиями).

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.  

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.eventMessage"
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
  "conversationIndex": "binary",
  "createdDateTime": "DateTimeOffset",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isAllDay": "Boolean",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "DateTimeOffset",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": {"@odata.type": "microsoft.graph.meetingMessageType"},
  "parentFolderId": "string",
  "receivedDateTime": "DateTimeOffset",
  "recurrence": {"@odata.type": "microsoft.graph.patternedrecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "DateTimeOffset",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "UnsubscribeData": "string",
  "UnsubscribeEnabled": true,
  "webLink": "string"
}

```

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bccRecipients|Коллекция [recipient](recipient.md)|Получатели скрытой копии сообщения.|
|body|[itemBody](itembody.md)|Текст сообщения. В формате HTML или текстовом формате.|
|bodyPreview|String|Первые 255 символов в тексте сообщения. В текстовом формате. |
|categories|Коллекция String|Категории, связанные с сообщением.|
|ccRecipients|Коллекция [recipient](recipient.md)|Получатели копии сообщения.|
|changeKey|String|Версия сообщения.|
|conversationId|String|Идентификатор беседы, к которой принадлежит электронное сообщение.|
|conversationIndex|Binary|Индекс беседы, к которой принадлежит электронное сообщение.|
|createdDateTime|DateTimeOffset|Дата и время создания сообщения.|
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|Время окончания собрания запрошенного.|
|flag|[followUpFlag](followupflag.md)|Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения сообщения.|
|from|[recipient](recipient.md)|Владелец почтового ящика и отправитель сообщения.|
|hasAttachments|Boolean|Указывает на наличие вложений в сообщении.|
|id|String||
|importance|String| Важность сообщения: `low`, `normal`, `high`.|
|inferenceClassification|String| Возможные значения: `focused`, `other`.|
|internetMessageHeaders | Коллекция [internetMessageHeader](internetmessageheader.md) | Коллекция заголовков сообщений, установленных по [RFC 5322](https://www.ietf.org/rfc/rfc5322.txt), которые содержат информацию о маршруте прохождения сообщения. Только для чтения.|
|internetMessageId |String |Идентификатор сообщения в формате, установленном документом [RFC5322](https://www.ietf.org/rfc/rfc5322.txt). |
|isAllDay |Boolean|Указывает, является ли событие длится весь день. Изменяет значения этого свойства требует настройки свойств **startDateTime** и **endDateTime** , а также события.|
|isDeliveryReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|isDraft|Boolean|Указывает, является ли сообщение черновиком. Сообщение считается черновиком, если оно еще не отправлено.|
|isOutOfDate|Boolean|Указывает ли этот запрос на собрание было выполнено устаревших последних запроса.|
|isRead|Boolean|Указывает, прочитано ли сообщение.|
|isReadReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сообщения.|
|location|[location](location.md)|Место собрания запрошенного.|
|meetingMessageType|String| Тип сообщения о событии: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTenativelyAccepted`, `meetingDeclined`.|
|parentFolderId|String|Уникальный идентификатор родительского ресурса mailFolder для сообщения.|
|receivedDateTime|DateTimeOffset|Дата и время получения сообщения.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Шаблон повторения запрошенные собрания.|
|replyTo|Коллекция [recipient](recipient.md)|Электронные адреса, которые необходимо использовать при ответе.|
|sender|[recipient](recipient.md)|Учетная запись, которая фактически используется для создания сообщения.|
|sentDateTime|DateTimeOffset|Дата и время отправки сообщения.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|Время начала запрошенные собрания.|
|subject|String|Тема сообщения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели сообщения, указанные в поле "Кому".|
|type|String|Тип запрошенного собрания: `singleInstance`, `occurence`, `exception`, `seriesMaster`.|
|uniqueBody|[itemBody](itembody.md)|Часть текста сообщения, которая является уникальной для текущего сообщения.|
|UnsubscribeData|String|Допустимые объекты, анализируемые из заголовка List-Unsubscribe  Это данные для почтовой команды в заголовке List-Unsubscribe, если свойству UnsubscribeEnabled присвоено значение true.|
|UnsubscribeEnabled|Boolean|Указывает, допускает ли сообщение отмену подписки.  Имеет значение True, если заголовок List-Unsubscribe соответствует документу RFC-2369.|
|webLink|String|URL-адрес для открытия сообщения в Outlook Web App.<br><br>Чтобы изменить способ отображения сообщения, можно добавить аргумент ispopout в конце URL-адреса. Если аргумент ispopout отсутствует или для него задано значение 1, то сообщение откроется во всплывающем окне. Если для аргумента ispopout задано значение 0, то в браузере сообщение будет отображаться в области просмотра Outlook Web App.<br><br>Сообщение откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook Web App. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br><br>Доступ к этому URL-адресу можно получить из объекта iFrame.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md)|Коллекция [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md)и [referenceAttachment](referenceattachment.md) вложений для сообщения. Только для чтения. Допускается значение null.|
|event|[event](event.md)| Событие, связанное с сообщением о событии. Для участников или ресурсов помещений предполагается, что помощник по ведению календаря настроен для автоматического обновления события в календаре, если поступают сообщения с приглашением на собрание. Свойство навигации.  Только для чтения.|
|extensions|Коллекция [extension](extension.md)| Коллекция открытых расширений, определенных для сообщения о событии. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для eventMessage. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для eventMessage. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение объекта eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Считывание свойств и отношений объекта eventMessage.|
|[Обновление](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Обновление объекта eventMessage.|
|[Удаление](../api/eventmessage-delete.md) | Нет |Удаление объекта eventMessage.|
|[copy](../api/message-copy.md)|[message](message.md)|Копирование сообщения в папку.|
|[createForward](../api/message-createforward.md)|[message](message.md)|Создание черновика сообщения для пересылки. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[createReply](../api/message-createreply.md)|[message](message.md)|Создание черновика для ответа. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[createReplyAll](../api/message-createreplyall.md)|[message](message.md)|Создание черновика сообщения для ответа всем пользователям. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[forward](../api/message-forward.md)|Нет|Пересылка сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[move](../api/message-move.md)|[message](message.md)|Перемещение сообщения в папку. При этом в целевой папке создается новая копия сообщения.|
|[reply](../api/message-reply.md)|Нет|Ответ отправителю сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[replyAll](../api/message-replyall.md)|Нет|Ответ всем получателям сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[send](../api/message-send.md)|Нет|Отправка ранее созданного черновика сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[unsubscribe](../api/message-unsubscribe.md)|Нет|Отправка сообщения, используя данные и адрес, указанные в это первой команде mailto заголовка List-Unsubscribe.|
|**Вложения**| | |
|[Список вложений](../api/eventmessage-list-attachments.md) |Коллекция [attachment](attachment.md)| Получение всех файлов, вложенных в сообщение о событии.|
|[Добавление вложения](../api/eventmessage-post-attachments.md) |[attachment](attachment.md)| Вложение в сообщение о событии нового файла путем публикации в коллекции вложений.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получите open расширения, определяется именем.|
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
  "description": "eventMessage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/eventmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
