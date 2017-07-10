<a id="configuring-the-invitation-message" class="xliff"></a>
# Настройка приглашения

Объект invitedUserMessageInfo позволяет настроить сообщение [приглашение](invitation.md).


<a id="properties" class="xliff"></a>
## Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ccRecipients|[Recipient](recipient.md)|Дополнительные получатели, которым следует отправить приглашение. В настоящее время поддерживается только 1 дополнительный получатель.|
|customizedMessageBody|Строка|Ваш собственный текст сообщения, который можно отправлять вместо предоставляемого по умолчанию.|
|messageLanguage|String|Выбранный вами язык для сообщения, которое отправляется по умолчанию. Если указано значение customizedMessageBody, это свойство игнорируется, и сообщение отправляется с помощью customizedMessageBody. Язык должен быть указан в формате ISO 639. Значение по умолчанию — en-US.|


<a id="json-representation" class="xliff"></a>
## Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
