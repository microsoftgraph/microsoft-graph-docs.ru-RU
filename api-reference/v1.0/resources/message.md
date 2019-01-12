---
title: Тип ресурса message
description: Сообщение в mailFolder.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: ea66839fe756fc6ecd57008c775fd20a9a23633a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966456"
---
# <a name="message-resource-type"></a>Тип ресурса message

Сообщение в mailFolder.

Этот ресурс поддерживает:

- Добавление собственных данных в качестве настраиваемых заголовков сообщений Интернета. Добавление пользовательских заголовков только при создании сообщения и назвать их начинающиеся с «x-». После отправки сообщения не может изменить заголовки. Чтобы получить заголовки сообщений, применение `$select` параметр в [сообщение](../api/message-get.md) операции запроса.
- Добавление данные как настраиваемые свойства в качестве [расширения](/graph/extensibility-overview).
- Подписка на [уведомления об изменении](/graph/webhooks).
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
|body|[itemBody](itembody.md)|Текст сообщения. Она может быть в формате HTML или текст. Узнайте о [безопасном HTML в тексте сообщения](/graph/outlook-create-send-messages#reading-messages-with-control-over-the-body-format-returned).|
|bodyPreview|String|Первые 255 символов в тексте сообщения. В текстовом формате.|
|categories|Коллекция String|Категории, сопоставленные с сообщением.|
|ccRecipients|Коллекция [recipient](recipient.md)|Получатели копии сообщения.|
|changeKey|String|Версия сообщения.|
|conversationId|String|Идентификатор беседы, к которой принадлежит электронное сообщение.|
|createdDateTime|DateTimeOffset|Дата и время создания сообщения.|
|flag|[followupFlag](followupflag.md)|Значение флага, которое указывает статус, дату начала, дату выполнения или дату завершения сообщения.|
|from|[recipient](recipient.md)|Владелец почтового ящика и отправитель сообщения. Значение должно соответствовать фактический почтового ящика, используемого. Узнать больше о [параметр из свойства отправителя и](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) сообщения.|
|hasAttachments|Boolean|Указывает на наличие вложений в сообщении. Это свойство не включает встроенные вложения, поэтому, если сообщение содержит только встроенные вложения, это свойство имеет значение false. Чтобы проверить наличие встроенных вложений, проанализируйте свойство **body** на наличие атрибута `src`, например `<IMG src="cid:image001.jpg@01D26CD8.6C05F070">`.|
|id|String|Уникальный идентификатор сообщения (обратите внимание, что это значение может меняться при перемещении и изменении сообщения).|
|importance|importance| Важность сообщения: `Low`, `Normal`, `High`.|
|inferenceClassification | inferenceClassificationType | Классификация сообщений для пользователя, на основе предполагаемых релевантность или важность, или явное переопределение. Возможные значения: `focused` или `other`. |
|internetMessageHeaders | Коллекция [internetMessageHeader](internetmessageheader.md) | Коллекция заголовки сообщений, определенные в [RFC5322](https://www.ietf.org/rfc/rfc5322.txt). Набор включает заголовки сообщений, указывая сетевой путь, по сообщение от отправителя получателю. Он также может содержать заголовки настраиваемого сообщения, в которых содержатся данные приложения для сообщения. |
|internetMessageId |String |Идентификатор сообщения в формате, установленном документом [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). |
|isDeliveryReceiptRequested|Логический|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|isDraft|Boolean|Указывает, является ли сообщение черновиком. Сообщение считается черновиком, если оно еще не отправлено.|
|isRead|Логический|Указывает, прочитано ли сообщение.|
|isReadReceiptRequested|Логический|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сообщения.|
|parentFolderId|String|Уникальный идентификатор родительского ресурса mailFolder для сообщения.|
|receivedDateTime|DateTimeOffset|Дата и время получения сообщения.|
|replyTo|Коллекция [recipient](recipient.md)|Электронные адреса, которые необходимо использовать при ответе.|
|sender|[recipient](recipient.md)|Учетная запись, которая фактически используется для создания сообщения. В большинстве случаев это значение — то же, что свойство **из** . Это свойство можно задать значение при отправке сообщения из [общего почтового ящика](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)или отправка сообщения [Делегирование](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926). В любом случае значение должно соответствовать фактический почтового ящика, используемого. Узнать больше о [параметр из свойства отправителя и](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) сообщения.|
|sentDateTime|DateTimeOffset|Дата и время отправки сообщения.|
|subject|String|Тема сообщения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели сообщения, указанные в поле "Кому".|
|uniqueBody|[itemBody](itembody.md)|Часть текста сообщения, которая уникальна для текущего сообщения. Экземпляр **uniqueBody** не возвращается по умолчанию, но может быть получен для заданного сообщения с помощью запроса `?$select=uniqueBody`. В формате HTML или текстовом формате.|
|webLink|String|URL-адрес для открытия сообщения в Outlook Web App.<br><br>Чтобы изменить способ отображения сообщения, можно добавить аргумент ispopout в конце URL-адреса. Если аргумент ispopout отсутствует или для него задано значение 1, то сообщение откроется во всплывающем окне. Если для аргумента ispopout задано значение 0, то в браузере сообщение будет отображаться в области просмотра Outlook Web App.<br><br>Сообщение откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook Web App. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br><br>Доступ к этому URL-адресу можно получить из объекта iFrame.|


## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md) |Вложения [fileAttachment](fileattachment.md) и [itemAttachment](itemattachment.md) для сообщения.|
|extensions|Коллекция [extension](extension.md)|Коллекция open расширения, определенные для сообщения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция Многозначный расширенных свойств, определенных для сообщения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенные свойства одно значение, определенное для сообщения. Допускается значение null.|

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
    "multiValueExtendedProperties"
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
