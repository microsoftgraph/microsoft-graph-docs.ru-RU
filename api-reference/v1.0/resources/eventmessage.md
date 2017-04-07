# <a name="eventmessage-resource-type"></a>Тип ресурса eventMessage

Сообщение, которое представляет собой приглашение на собрание, оповещение о принятии (в том числе предварительном) или отклонении такого приглашения, оповещение об отмене собрания.

Сообщение о событии EventMessage обычно находится в папке "Входящие". Туда оно попадает, если организатор события создает собрание, или если участник отвечает на приглашение на собрание. В случае сообщений о событии вы действуете так же, как в случае объекта Message, но с некоторыми незначительными отличиями, описанными в приведенной ниже таблице.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение объекта eventMessage](../api/eventmessage_get.md) | [eventMessage](eventmessage.md) |Считывание свойств и отношений объекта eventMessage.|
|[Обновление](../api/eventmessage_update.md) | [eventMessage](eventmessage.md)  |Обновление объекта eventMessage. |
|[Удаление](../api/message_delete.md) | Нет |Удаление объекта eventMessage. |
|[copy](../api/message_copy.md)|[Message](message.md)|Копирование сообщения в папку.|
|[createForward](../api/message_createforward.md)|[Message](message.md)|Создание черновика пересылаемого сообщения. После этого вы сможете [обновить](../api/message_update.md) или [отправить](../api/message_send.md) черновик.|
|[createReply](../api/message_createreply.md)|[Message](message.md)|Создание черновика ответного сообщения. После этого вы сможете [обновить](../api/message_update.md) или [отправить](../api/message_send.md) черновик.|
|[createReplyAll](../api/message_createreplyall.md)|[Message](message.md)|Создание черновика сообщения для ответа всем пользователям. После этого вы сможете [обновить](../api/message_update.md) или [отправить](../api/message_send.md) черновик.|
|[forward](../api/message_forward.md)|Нет|Пересылка сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[move](../api/message_move.md)|[Message](message.md)|Перемещение сообщения в папку. При этом в целевой папке создается новая копия сообщения.|
|[reply](../api/message_reply.md)|Нет|Ответ отправителю сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[replyAll](../api/message_replyall.md)|Нет|Ответ всем получателям сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|[send](../api/message_send.md)|Нет|Отправка ранее созданного черновика сообщения. После этого сообщение сохраняется в папке "Отправленные".|
|**Вложения**| | |
|[Список вложений](../api/eventmessage_list_attachments.md) |Коллекция [Attachment](attachment.md)| Получение всех вложений для eventMessage.|
|[Добавление вложения](../api/eventmessage_post_attachments.md) |[Attachment](attachment.md)| Добавление нового вложения для eventMessage путем публикации в коллекции вложений.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension_get.md) |Коллекция [openTypeExtension](opentypeextension.md)| Получение объекта или объектов открытого расширения, которые определяются по имени или полному имени.|
|**Расширенные свойства**| | |
|[Создание однозначного расширенного свойства](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[eventMessage](eventMessage.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем экземпляре eventMessage.   |
|[Получение eventMessage с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty_get.md)  | [eventMessage](eventMessage.md) | Получение экземпляров eventMessage, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [eventMessage](eventMessage.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре eventMessage.  |
|[Получение eventMessage с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty_get.md)  | [eventMessage](eventMessage.md) | Получение eventMessage, которое содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |


## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|bccRecipients|Коллекция [recipient](recipient.md)|Получатели скрытой копии сообщения.|
|body|[itemBody](itembody.md)|Текст сообщения.|
|bodyPreview|String|Первые 255 символов в тексте сообщения.|
|categories|Коллекция String|Категории, сопоставленные с сообщением.|
|ccRecipients|Коллекция [recipient](recipient.md)|Получатели копии сообщения.|
|changeKey|String|Версия сообщения.|
|conversationId|String|Идентификатор беседы, к которой принадлежит электронное сообщение.|
|createdDateTime|DateTimeOffset|Дата и время создания сообщения.|
|from|[recipient](recipient.md)|Владелец почтового ящика и отправитель сообщения.|
|hasAttachments|Boolean|Указывает на наличие вложений в сообщении.|
|id|String||
|importance|String| Важность сообщения: `Low`, `Normal`, `High`.|
|internetMessageId |String |Идентификатор сообщения в формате, установленном документом [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). |
|isDeliveryReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|isDraft|Логическое|Указывает, является ли сообщение черновиком. Сообщение считается черновиком, если оно еще не отправлено.|
|isRead|Boolean|Указывает, прочитано ли сообщение.|
|isReadReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сообщения.|
|meetingMessageType|String| Тип сообщения о событии: `None`, `MeetingRequest`, `MeetingCancelled`, `MeetingAccepted`, `MeetingTenativelyAccepted`, `MeetingDeclined`.|
|parentFolderId|String|Уникальный идентификатор родительского ресурса mailFolder для сообщения.|
|receivedDateTime|DateTimeOffset|Дата и время получения сообщения.|
|replyTo|Коллекция [recipient](recipient.md)|Электронные адреса, которые необходимо использовать при ответе.|
|sender|[recipient](recipient.md)|Учетная запись, которая фактически используется для создания сообщения.|
|sentDateTime|DateTimeOffset|Дата и время отправки сообщения.|
|subject|String|Тема сообщения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели сообщения, указанные в поле "Кому".|
|uniqueBody|[itemBody](itembody.md)|Часть текста сообщения, которая является уникальной для текущего сообщения.|
|webLink|String|URL-адрес для открытия сообщения в Outlook Web App.<br><br>Чтобы изменить способ отображения сообщения, можно добавить аргумент ispopout в конце URL-адреса. Если аргумент ispopout отсутствует или для него задано значение 1, то сообщение откроется во всплывающем окне. Если для аргумента ispopout задано значение 0, то в браузере сообщение будет отображаться в области просмотра Outlook Web App.<br><br>Сообщение откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook Web App. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br><br>Доступ к этому URL-адресу можно получить из объекта iFrame.|


## <a name="relationships"></a>Отношения
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [Attachment](attachment.md)| Только для чтения. Допускается значение null.|
|событие|[Event](event.md)| Событие, связанное с сообщением о событии. Для участников или ресурсов помещений предполагается, что помощник по ведению календаря настроен для автоматического обновления события в календаре, если поступают сообщения с приглашением на собрание. Свойство навигации.  Только для чтения.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для eventMessage. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для eventMessage. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для eventMessage. Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.  

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.eventmessage"
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
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "meetingMessageType": "String",
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
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
