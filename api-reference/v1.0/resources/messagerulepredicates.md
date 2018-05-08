# <a name="messagerulepredicates-resource-type"></a>Тип ресурса messageRulePredicates


Представляет набор условий и исключений, доступных для правила.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| bodyContains | Коллекция (String) | Представляет строки, которые должны 	присутствовать в тексте входящего сообщения, чтобы применялось условие или исключение. |
| bodyOrSubjectContains | Коллекция (String) | Представляет строки, которые должны присутствовать в тексте или теме входящего сообщения, чтобы применялось условие или исключение. |
| categories | Коллекция (String) | Представляет категории, к которым должно относиться входящее сообщение, чтобы применялось условие или исключение. |
| fromAddresses | Коллекция ([recipient](recipient.md)) | Представляет электронные адреса конкретных отправителей, при наличии которых ко входящему сообщению применяется условие или исключение. |
| hasAttachments | Boolean | Указывает, должно ли входящее сообщение содержать вложения, чтобы применялось условие или исключение. |
| headerContains | Коллекция (String) | Представляет строки, которые должны присутствовать в заголовках входящего сообщения, чтобы применялось условие или исключение. |
| importance | String | Уровень важности, который должен быть задан для входящего сообщения, чтобы применялось условие или исключение: `low`, `normal`, `high`. |
| isApprovalRequest | Boolean | Указывает, должно ли входящее сообщение быть запросом утверждения, чтобы применялось условие или исключение. |
| isAutomaticForward | Boolean | Указывает, должно ли входящее сообщение быть автоматически пересланным, чтобы применялось условие или исключение. |
| isAutomaticReply | Boolean | Указывает, должно ли входящее сообщение быть автоматическим ответом, чтобы применялось условие или исключение. |
| isEncrypted | Boolean | Указывает, должно ли входящее сообщение быть зашифровано, чтобы применялось условие или исключение. |
| isMeetingRequest | Boolean | Указывает, должно ли входящее сообщение быть приглашением на собрание, чтобы применялось условие или исключение. |
| isMeetingResponse | Boolean | Указывает, должно ли входящее сообщение быть ответом на приглашение на собрание, чтобы применялось условие или исключение. |
| isNonDeliveryReport | Boolean | Указывает, должно ли входящее сообщение быть отчетом о недоставке, чтобы применялось условие или исключение. |
| isPermissionControlled | Boolean | Указывает, должно ли быть включено управление разрешениями (защита RMS) для входящего сообщения, чтобы к нему применялось условие или исключение. |
| isReadReceipt | Boolean | Указывает, должно ли входящее сообщение быть уведомлением о прочтении, чтобы применялось условие или исключение. |
| isSigned | Boolean | Указывает, должно ли входящее сообщение иметь подпись S/MIME, чтобы применялось условие или исключение. |
| isVoicemail | Boolean | Указывает, должно ли входящее сообщение быть сообщением голосовой почты, чтобы к нему применялось условие или исключение. |
| messageActionFlag | String  | Представляет значение флага для действия, которое должно присутствовать во входящем сообщении, чтобы к нему применялось условие или исключение. Возможные значения: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`. |
| notSentToMe | Boolean | Указывает, должно ли условие или исключение применяться только в том случае, если владелец почтового ящика не является получателем входящего сообщения. |
| recipientContains | Коллекция (String) | Представляет строки, которые должны присутствовать в свойстве **toRecipients** или **ccRecipients** входящего сообщения, чтобы к нему применялось условие или исключение. |
| senderContains | Коллекция (String) | Представляет строки, которые должны присутствовать в свойстве **from** входящего сообщения, чтобы к нему применялось условие или исключение. |
| sensitivity | String | Представляет уровень конфиденциальности, который должен быть задан для входящего сообщения, чтобы к нему применялось условие или исключение. Возможные значения: `normal`, `personal`, `private`, `confidential`. |
| sentCcMe | Boolean | Указывает, должен ли владелец почтового ящика быть указан в свойстве **ccRecipients** входящего сообщения, чтобы применялось условие или исключение. |
| sentOnlyToMe | Boolean | Указывает, должен ли владелец почтового ящика быть единственным получателем входящего сообщения, чтобы применялось условие или исключение. |
| sentToAddresses | Коллекция ([recipient](recipient.md)) | Представляет электронные адреса, на которые должно быть отправлено входящее сообщение, чтобы к нему применялось условие или исключение. |
| sentToMe | Boolean | Указывает, должен ли владелец почтового ящика быть указан в свойстве **toRecipients** входящего сообщения, чтобы применялось условие или исключение. |
| sentToOrCcMe | Boolean | Указывает, должен ли владелец почтового ящика быть указан в свойстве **toRecipients** или **ccRecipients** входящего сообщения, чтобы применялось условие или исключение. |
| subjectContains | Коллекция (String) | Представляет строки, которые должны присутствовать в теме входящего сообщения, чтобы к нему применялось условие или исключение. |
| withinSizeRange | [sizeRange](sizerange.md) | Представляет минимальное и максимальное значения (в килобайтах), между которыми должен находиться размер входящего сообщения, чтобы применялось условие или исключение. |



## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRulePredicates"
}-->

```json
{
  "bodyContains": ["String"],
  "bodyOrSubjectContains": ["String"],
  "categories": ["String"],
  "fromAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": "Boolean",
  "headerContains": ["String"],
  "importance": "String",
  "isApprovalRequest": "Boolean",
  "isAutomaticForward": "Boolean",
  "isAutomaticReply": "Boolean",
  "isEncrypted": "Boolean",
  "isMeetingRequest": "Boolean",
  "isMeetingResponse": "Boolean",
  "isNonDeliveryReport": "Boolean",
  "isPermissionControlled": "Boolean",
  "isReadReceipt": "Boolean",
  "isSigned": "Boolean",
  "isVoicemail": "Boolean",
  "messageActionFlag": "String",
  "notSentToMe": "Boolean",
  "recipientContains": ["String"],
  "senderContains": ["String"],
  "sensitivity": "String",
  "sentCcMe": "Boolean",
  "sentOnlyToMe": "Boolean",
  "sentToAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "sentToMe": "Boolean",
  "sentToOrCcMe": "Boolean",
  "subjectContains": ["String"],
  "withinSizeRange": {"@odata.type": "microsoft.graph.sizeRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->