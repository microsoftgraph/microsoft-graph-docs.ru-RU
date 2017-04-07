# <a name="message-resource-type"></a>Тип ресурса message

Сообщение в mailFolder.

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](../../../concepts/extensibility_overview.md).


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список сообщений](../api/user_list_messages.md) |Коллекция [message](message.md) | Получение всех сообщений в почтовом ящике пользователя, выполнившего вход (в том числе сообщений в папках "Удаленные" и "Несрочные"). |
|[Создание сообщения](../api/user_post_messages.md) | [message](message.md) | [Создание](../api/user_post_messages.md#request-1) черновика нового сообщения. |
|[Получение сообщения](../api/message_get.md) | [message](message.md) |Считывание свойств и отношений объекта message.|
|[Обновление](../api/message_update.md) | [message](message.md) |Обновление объекта message.|
|[Удаление](../api/message_delete.md) | Нет |Удаление объекта message. |
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
|[Список вложений](../api/message_list_attachments.md) |Коллекция [Attachment](attachment.md)| Получает все вложения сообщения.|
|[Добавление вложения](../api/message_post_attachments.md) |[Attachment](attachment.md)| Добавление нового вложения к сообщению путем публикации в коллекции вложений.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension_get.md) |Коллекция [openTypeExtension](opentypeextension.md)| Получение объекта или объектов открытого расширения, которые определяются по имени или полному имени.|
|**Расширенные свойства**| | |
|[Создание однозначного расширенного свойства](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[message](message.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем сообщении.   |
|[Получение сообщения с однозначным расширенным свойством](../api/singlevaluelegacyextendedproperty_get.md)  | [message](message.md) | Получение сообщений, которые содержат однозначное расширенное свойство, с помощью `$expand` или `$filter`. |
|[Создание многозначного расширенного свойства](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [message](message.md) | Создание одного или нескольких многозначных расширенных свойств в новом или существующем сообщении.  |
|[Получение сообщения с многозначным расширенным свойством](../api/multivaluelegacyextendedproperty_get.md)  | [message](message.md) | Получение сообщения, которое содержит многозначное расширенное свойство, с помощью `$expand`. |


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
|id|String|Уникальный идентификатор сообщения (обратите внимание, что это значение может меняться при перемещении и изменении сообщения).|
|importance|String| Важность сообщения: `Low`, `Normal`, `High`.|
|inferenceClassification | String | Классификация сообщения для пользователя на основании подразумеваемой релевантности или важности либо явного переопределения. Возможные значения: `focused` или `other`. |
|internetMessageId |String |Идентификатор сообщения в формате, установленном документом [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). |
|isDeliveryReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|isDraft|Логическое|Указывает, является ли сообщение черновиком. Сообщение считается черновиком, если оно еще не отправлено.|
|isRead|Boolean|Указывает, прочитано ли сообщение.|
|isReadReceiptRequested|Boolean|Указывает, запрашивается ли уведомление о прочтении сообщения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сообщения.|
|parentFolderId|String|Уникальный идентификатор родительского ресурса mailFolder для сообщения.|
|receivedDateTime|DateTimeOffset|Дата и время получения сообщения.|
|replyTo|Коллекция [recipient](recipient.md)|Электронные адреса, которые необходимо использовать при ответе.|
|sender|[recipient](recipient.md)|Учетная запись, которая фактически используется для создания сообщения.|
|sentDateTime|DateTimeOffset|Дата и время отправки сообщения.|
|subject|String|Тема сообщения.|
|toRecipients|Коллекция [recipient](recipient.md)|Получатели сообщения, указанные в поле "Кому".|
|uniqueBody|[itemBody](itembody.md)|Часть текста сообщения, которая уникальна для текущего сообщения. Экземпляр uniqueBody не предоставляется по умолчанию, но может быть получен для заданного сообщения с помощью такого запроса: ?$select=uniqueBody.|
|webLink|String|URL-адрес для открытия сообщения в Outlook Web App.<br><br>Чтобы изменить способ отображения сообщения, можно добавить аргумент ispopout в конце URL-адреса. Если аргумент ispopout отсутствует или для него задано значение 1, то сообщение откроется во всплывающем окне. Если для аргумента ispopout задано значение 0, то в браузере сообщение будет отображаться в области просмотра Outlook Web App.<br><br>Сообщение откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook Web App. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br><br>Доступ к этому URL-адресу можно получить из объекта iFrame.|

**Удаление сценария из свойства Body**

Текст сообщения может быть представлен в формате HTML или в виде обычного текста. Если текст представлен в формате HTML, то по умолчанию любой потенциально небезопасный код HTML (например, JavaScript), внедренный в свойство Body, удаляется, прежде чем содержимое сообщения возвращается в отклике REST. Чтобы получить все исходное содержимое в формате HTML, добавьте следующий заголовок HTTP-запроса:
```
Prefer: outlook.allow-unsafe-html
```

**Задание свойств From и Sender**

В большинстве случаев при создании сообщения свойства From и Sender представляют одного вошедшего пользователя, если ни одно из них не было обновлено, как описано ниже.

- Свойство **From** можно изменить, если администратор Exchange назначил другим пользователям права **SendAs** для почтового ящика. Для этого администратор может назначить владельца, выбрав элемент **Разрешения для почтового ящика** на портале управления Azure, либо использовать Центр администрирования Exchange или командлет Add-ADPermission в Windows PowerShell. Затем вы можете задать в коде свойство **From** для одного из пользователей, обладающих правами **SendAs** для этого почтового ящика.
- Свойство **Sender** можно изменить, если владелец почтового ящика предоставил одному или нескольким пользователям права на отправку сообщений из этого почтового ящика. Владелец почтового ящика может делегировать разрешения в Outlook. Когда представитель отправляет сообщение от имени владельца почтового ящика, в свойстве **Sender** указывается учетная запись представителя, а в свойстве **From** — владелец почтового ящика. Вы можете задать в коде свойство **Sender** для пользователя, обладающего правами представителя для этого почтового ящика.

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md) |Вложения [fileAttachment](fileattachment.md) и [itemAttachment](itemattachment.md) для сообщения.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для сообщения. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция многозначных расширенных свойств, определенных для сообщения. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция однозначных расширенных свойств, определенных для сообщения. Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message"
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
  "inferenceClassification": "String",
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
  "webLink": "string"
}

```

## <a name="see-also"></a>См. также

- [Получение параметров почтового ящика](../api/user_get_mailboxsettings.md) 
- [Обновление параметров почтового ящика](../api/user_update_mailboxsettings.md)
- [Добавление пользовательских данных в ресурсы с помощью расширений](../../../concepts/extensibility_overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](../../../concepts/extensibility_open_users.md)
- [Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
