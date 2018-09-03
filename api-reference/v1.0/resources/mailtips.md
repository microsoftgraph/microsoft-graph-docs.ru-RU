# <a name="mailtips-resource-type"></a>Тип ресурса mailTips

Информационные сообщения о получателе, отображаемые для пользователей при составлении сообщения. Например, сообщение об отсутствии на рабочем месте, отправляемое получателем сообщения в качестве автоматического ответа.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Подсказки для автоматического ответа, если он настроен получателем. |
| customMailTip | String (строка) | Настраиваемая подсказка, которую можно настроить для почтового ящика получателя. |
| deliveryRestricted| Boolean (логический) | Указывает, ограничен ли почтовый ящик получателя, например, с приемом сообщений только от предопределенного списка отправителей, отклонением сообщений от предопределенного списка отправителей или приемом сообщений только от отправителей, прошедших проверку подлинности. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | Адрес электронной почты получателя для получения подсказок. |
| error | [mailTipsError](../resources/mailtipserror.md) | Ошибки, возникающие во время действия [GetMailTips](../api/user_getmailtips.md). |
| externalMemberCount | Int32 | Количество внешних участников, если получатель является списком рассылки. |
| isModerated |Boolean (логический)  | Указывает, требуется ли утверждение отправки сообщений получателю. Например, для случаев, когда получатель представляет собой большой список рассылки, а модератор настроен для утверждения сообщений, отправленных в этот список рассылки, или когда отправка сообщений получателю требует утверждения менеджером получателя. |
| mailboxFull | Boolean (логический) | Переполненность почтового ящика получателя. |
| maxMessageSize | Int32 | Максимальный размер сообщения, который настроен для организации или почтового ящика получателя. |
| recipientScope | String (строка) | Область получателя. Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`. Например, администратор может назначить другую организацию своим "партнером". Область полезна, если администратор желает, чтобы определенные подсказки были доступны для определенных областей. Она также полезна для отправителей: они информируются о том, что их сообщение может покинуть пределы организации, что позволяет им пересмотреть формулировку, тон и содержимое сообщения.|
| recipientSuggestions | Коллекция [recipient](../resources/recipient.md) | Предложения получателей, которые основываются на предыдущем контексте, когда они фигурируют в таком же сообщении. |
| totalMemberCount | Int32 | Число участников, если получатель является списком рассылки. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->