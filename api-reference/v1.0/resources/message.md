---
title: Тип ресурса message
description: Сообщение в mailFolder.
author: svpsiva
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e0957e7f62cacd83d6ab064dfae7fb50a3f932e5
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563676"
---
# <a name="message-resource-type"></a>Тип ресурса message

Пространство имен: microsoft.graph

Сообщение в mailFolder.

Максимальное число получателей, включенное в свойства **toRecipients**, **ccRecipients** и **bccRecipients** для одного сообщения электронной почты, отправляемого из почтового ящика Exchange Online, равно 500. Дополнительные сведения см. в разделе [Ограничения на отправку](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits).

Этот ресурс поддерживает:

- добавление собственных данных как настраиваемых заголовков сообщений Интернета. Добавляйте настраиваемые заголовки только при создании сообщения и выбирайте для них имя, начинающееся с "x-". После отправки сообщения невозможно изменить заголовки. Чтобы получить заголовки сообщения, примените параметр запроса `$select` в операции [получения сообщения](../api/message-get.md);
- добавление собственных данных как настраиваемых свойств в виде [расширений](/graph/extensibility-overview);
- подписку на [уведомления об изменениях](/graph/webhooks);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/message-delta.md)).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список сообщений](../api/user-list-messages.md) |Коллекция [message](message.md) | Получение всех сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные"). |
|[Создание сообщения](../api/user-post-messages.md) | [message](message.md) | [Создание](../api/user-post-messages.md#request-1) черновика нового сообщения. |
|[Получение сообщения](../api/message-get.md) | [message](message.md) |Считывание свойств и отношений объекта message.|
|[Обновление](../api/message-update.md) | [message](message.md) |Обновление объекта message.|
|[Удаление](../api/message-delete.md) | Нет |Удаление объекта message. |
|[copy](../api/message-copy.md)|[Message](message.md)|Копирование сообщения в папку.|
|[createForward](../api/message-createforward.md)|[Message](message.md)|Создание черновика пересылаемого сообщения. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[createReply](../api/message-createreply.md)|[Message](message.md)|Создание черновика ответного сообщения. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[createReplyAll](../api/message-createreplyall.md)|[Message](message.md)|Создание черновика сообщения для ответа всем пользователям. После этого вы сможете [обновить](../api/message-update.md) или [отправить](../api/message-send.md) черновик.|
|[delta](../api/message-delta.md)|Коллекция объектов [message](message.md)| Получение списка сообщений, которые были добавлены в указанную папку, обновлены в ней или удалены из нее.|
|[forward](../api/message-forward.md)|Нет|Пересылка сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[move](../api/message-move.md)|[Message](message.md)|Перемещение сообщения в папку. При этом в целевой папке создается новая копия сообщения.|
|[reply](../api/message-reply.md)|Нет|Ответ отправителю сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[replyAll](../api/message-replyall.md)|Нет|Ответ всем получателям сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[send](../api/message-send.md)|Нет|Отправка ранее созданного черновика сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|**Вложения**| | |
|[Список вложений](../api/message-list-attachments.md) |Коллекция [Attachment](attachment.md)| Получает все вложения сообщения.|
|[Добавление вложения](../api/message-post-attachments.md) |[Attachment](attachment.md)| Добавление нового вложения к сообщению путем публикации в коллекции вложений.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция [openTypeExtension](opentypeextension.md)| Получение объектов открытого расширения, которые определяются по имени или полному имени.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Расширенные свойства**| | |
|[Создание однозначного расширенного свойства](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[message](message.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем сообщении.   |
|[Получение сообщения с однозначным расширенным свойством](../api/singlevaluelegacyextendedproperty-get.md)  | [message](message.md) | Получение сообщений, которые содержат однозначное расширенное свойство, с помощью `$expand` или `$filter`. |
|[Создание многозначного расширенного свойства](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [message](message.md) | Создание одного или нескольких многозначных расширенных свойств в новом или существующем сообщении.  |
|[Получение сообщения с многозначным расширенным свойством](../api/multivaluelegacyextendedproperty-get.md)  | [message](message.md) | Получение сообщения, которое содержит многозначное расширенное свойство, с помощью `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bccRecipients|Коллекция [recipient](recipient.md)|Получатели скрытой копии сообщения.|
|body|[itemBody](itembody.md)|Текст сообщения. В формате HTML или текстовом формате. Сведения о [надежном формате HTML в тексте сообщения](/graph/outlook-create-send-messages#reading-messages-with-control-over-the-body-format-returned).|
|bodyPreview|String|Первые 255 символов в тексте сообщения. В текстовом формате.|
|categories|Коллекция String|Категории, сопоставленные с сообщением.|
|ccRecipients|Коллекция [recipient](recipient.md)|Получатели копии сообщения.|
|changeKey|String|Версия сообщения.|
|conversationId|String|Идентификатор беседы, к которой принадлежит электронное сообщение.|
|conversationIndex|Edm.Binary|Указывает место сообщения в беседе.|
|createdDateTime|DateTimeOffset|Дата и время создания сообщения. <br><br> Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|
|flag|[followupFlag](followupflag.md)|Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения сообщения.|
|from|[recipient](recipient.md)|Владелец почтового ящика, из которого отправлено сообщение. В большинстве случаев это значение совпадает со свойством **sender**, кроме сценариев предоставления общего доступа или делегирования. Значение должно соответствовать фактически используемому почтовому ящику. Дополнительные сведения о [задании свойств from и sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) сообщения.|
|hasAttachments|Boolean|Указывает на наличие вложений в сообщении. Это свойство не включает встроенные вложения, поэтому, если сообщение содержит только встроенные вложения, это свойство имеет значение false. Чтобы проверить наличие встроенных вложений, проанализируйте свойство **body** на наличие атрибута `src`, например `<IMG src="cid:image001.jpg@01D26CD8.6C05F070">`.|
|id|String|Уникальный идентификатор сообщения (обратите внимание, что это значение может меняться при перемещении и изменении сообщения).|
|importance|importance| Важность сообщения: `Low`, `Normal`, `High`.|
|inferenceClassification | inferenceClassificationType | Классификация сообщения для пользователя на основании подразумеваемой релевантности или важности либо явного переопределения. Допустимые значения: `focused` или `other`. |
|internetMessageHeaders | Коллекция [internetMessageHeader](internetmessageheader.md) | Коллекция заголовков сообщений, определенных документом [RFC5322](https://www.ietf.org/rfc/rfc5322.txt). Набор содержит заголовки сообщений, указывающие сетевой путь, пройденный сообщением от отправителя до получателя. Он также может содержать настраиваемые заголовки сообщений, содержащие данные приложения для сообщения. <br><br> Возвращается только при применении параметра запроса `$select`. Только для чтения. |
|internetMessageId |String |Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). |
|isDeliveryReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|isDraft|Логическое|Указывает, является ли сообщение черновиком. Сообщение считается черновиком, если оно еще не отправлено.|
|isRead|Boolean|Указывает, прочитано ли сообщение.|
|isReadReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сообщения. <br><br> Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|
|parentFolderId|String|Уникальный идентификатор родительского ресурса mailFolder для сообщения.|
|receivedDateTime|DateTimeOffset|Дата и время получения сообщения. <br><br> Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|
|replyTo|Коллекция [recipient](recipient.md)|Электронные адреса, которые необходимо использовать при ответе.|
|sender|[recipient](recipient.md)|Учетная запись, которая фактически используется для создания сообщения. В большинстве случаев это значение совпадает со значением свойства **from**. Этому свойству можно присвоить другое значение при отправке сообщения из [общего почтового ящика](/exchange/collaboration/shared-mailboxes/shared-mailboxes), [для общего календаря или в качестве делегата](/graph/outlook-share-delegate-calendar.md). В любом случае значение должно соответствовать фактически используемому почтовому ящику. Дополнительные сведения о [задании свойств from и sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) сообщения.|
|sentDateTime|DateTimeOffset|Дата и время отправки сообщения. <br><br> Сведения о времени и дате представлены в формате ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".|
|subject|String|Тема сообщения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели сообщения, указанные в поле "Кому".|
|uniqueBody|[itemBody](itembody.md)|Часть текста сообщения, которая уникальна для текущего сообщения. Экземпляр **uniqueBody** не возвращается по умолчанию, но может быть получен для заданного сообщения с помощью запроса `?$select=uniqueBody`. В формате HTML или текстовом формате.|
|webLink|String|URL-адрес для открытия сообщения в Outlook в Интернете.<br><br>Чтобы изменить способ отображения сообщения, можно добавить аргумент ispopout в конце URL-адреса. Если аргумент ispopout отсутствует или для него задано значение 1, то сообщение откроется во всплывающем окне. Если для аргумента ispopout задано значение 0, то в браузере сообщение будет отображаться в области просмотра Outlook в Интернете.<br><br>Сообщение откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br><br>Доступ к этому URL-адресу невозможно получить из объекта iFrame.|


## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md) |Вложения [fileAttachment](fileattachment.md) и [itemAttachment](itemattachment.md) для сообщения.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для сообщения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция многозначных расширенных свойств, определенных для сообщения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция однозначных расширенных свойств, определенных для сообщения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties",

    "internetMessageHeaders"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
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
  "createdDateTime": "String (timestamp)",
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string",

  "attachments": [{"@odata.type": "microsoft.graph.attachment"}],
  "extensions": [{"@odata.type": "microsoft.graph.extension"}],
  "multiValueExtendedProperties": [{"@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"}],
  "singleValueExtendedProperties": [{"@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"}]
}

```

## <a name="see-also"></a>См. также

- [Получение параметров почтового ящика](../api/user-get-mailboxsettings.md)
- [Обновление параметров почтового ящика](../api/user-update-mailboxsettings.md)
- [Отслеживание изменений данных Microsoft Graph с помощью запроса изменений](/graph/delta-query-overview)
- [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages)
- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

