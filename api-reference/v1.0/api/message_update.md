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
| Авторизация  | строка  | Bearer {токен}. Обязательный. |
| Content-Type | строка  | Характер данных в теле объекта. Обязательный. |
## <a name="request-body"></a>Текст запроса
В основном тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, доступные для записи и обновления.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|bccRecipients|Получатель|Получатели скрытой копии сообщения. Обновляемые только если Draft = true.|
|категории|Коллекция String|Категории, сопоставленные с сообщением.|
|ccRecipients|Коллекция получателей|Получатели копии сообщения. Updatable only if isDraft = true.|
|from|Получатель|Владелец почтового ящика и отправитель сообщения. Updatable only if isDraft = true. Должно соответствовать фактически используемому почтовому ящику.|
|importance|Строка|Важность сообщения. Возможные значения: `Low`, `Normal`, `High`.|
|inferenceClassification | Строка | Классификация сообщения для пользователя на основе подразумеваемой релевантности или важности либо явного переопределения. Возможные значения: `focused` или`other`. |
|internetMessageId |Строка |Идентификатор сообщения в формате, установленном документом [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Обновляемые только если Draft = true.|
|isRead|Boolean|Указывает, прочитано ли сообщение.|
|replyTo|Коллекция получателей|Электронные адреса, которые необходимо использовать при ответе. Updatable only if isDraft = true.|
|отправитель|Получатель|Учетная запись, которая фактически используется для создания сообщения. Обновляемые только если isDraft = true, а также во время отправки сообщения из [общего почтового ящика](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)или отправки сообщения как [Делегат](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926). В любом случае, значение должно соответствовать фактически используемому почтовому ящику.|
|toRecipients|Коллекция получателей|Получатели сообщения, указанные в поле "Кому". Updatable only if isDraft = true.|
|текст сообщения|ItemBody|Текст сообщения. Updatable only if isDraft = true.|
|isDeliveryReceiptRequested|Boolean|Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.|
|isReadReceiptRequested|Boolean|Указывает, необходимо ли запрашивать уведомление о прочтении сообщения.|
|subject|Строка|Тема сообщения. Updatable only if isDraft = true.|

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
