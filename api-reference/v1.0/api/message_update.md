# <a name="update-message"></a>Обновление сообщения

Обновление свойств объекта сообщения.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Mail.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Mail.ReadWrite    |
|Для приложений | Mail.ReadWrite |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type | string  | Характер данных в теле объекта. Обязательный. |
## <a name="request-body"></a>Тело запроса
В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bccRecipients|Область записи|Получатели скрытой копии сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.|
|categories|Коллекция String|Категории, сопоставленные с сообщением.|
|ccRecipients|Коллекция объектов Recipient|Получатели копии сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.|
|from|Область записи|Владелец почтового ящика и отправитель сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.|
|importance|String|Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.|
|inferenceClassification | String | Классификация сообщения для пользователя на основании подразумеваемой релевантности или важности либо явного переопределения. Возможные значения: `focused` или `other`. |
|internetMessageId |Строка |Идентификатор сообщения в формате, определенном в документе [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Это свойство можно обновить, только если параметр IsDraft имеет значение true.|
|isRead|Boolean|Указывает, прочитано ли сообщение.|
|replyTo|Коллекция объектов Recipient|Электронные адреса, которые необходимо использовать при ответе. Это свойство можно обновить, только если параметр IsDraft имеет значение true.|
|sender|Область записи|Учетная запись, которая фактически используется для создания сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.|
|toRecipients|Коллекция объектов Recipient|Получатели сообщения, указанные в поле "Кому". Это свойство можно обновить, только если параметр IsDraft имеет значение true.|
|Основной текст|ItemBody|Текст сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.|
|isDeliveryReceiptRequested|Boolean|Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.|
|isReadReceiptRequested|Boolean|Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.|
|subject|String|Тема сообщения. Это свойство можно обновить, только если параметр IsDraft имеет значение true.|

Так как ресурс **message** поддерживает [расширения](../../../concepts/extensibility_overview.md), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **message**.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [message](../resources/message.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](../../../concepts/extensibility_overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
