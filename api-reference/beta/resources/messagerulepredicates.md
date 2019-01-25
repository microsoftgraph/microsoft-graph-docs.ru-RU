---
title: Тип ресурса messageRulePredicates
description: Представляет набор условий и исключений, доступных для правила.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fda6a160d30dc0d822f2e0aeb5642250d6b69658
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519439"
---
# <a name="messagerulepredicates-resource-type"></a>Тип ресурса messageRulePredicates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор условий и исключений, доступных для правила.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| bodyContains | Коллекция (String) | Представляет строки, которые должны 	присутствовать в тексте входящего сообщения, чтобы применялось условие или исключение. |
| bodyOrSubjectContains | Коллекция (String) | Представляет строки, которые должны присутствовать в тексте или теме входящего сообщения, чтобы применялось условие или исключение. |
| categories | Коллекция (String) | Представляет категории, к которым должно относиться входящее сообщение, чтобы применялось условие или исключение. |
| fromAddresses | Коллекция ([recipient](recipient.md)) | Представляет электронные адреса конкретных отправителей, при наличии которых ко входящему сообщению применяется условие или исключение. |
| hasAttachments | Логическое | Указывает, должно ли входящее сообщение содержать вложения, чтобы применялось условие или исключение. |
| headerContains | Коллекция (String) | Представляет строки, которые должны присутствовать в заголовках входящего сообщения, чтобы применялось условие или исключение. |
| importance | Строка | Уровень важности, который должен быть задан для входящего сообщения, чтобы применялось условие или исключение: `low`, `normal`, `high`. |
| isApprovalRequest | Логическое | Указывает, должно ли входящее сообщение быть запросом утверждения, чтобы применялось условие или исключение. |
| isAutomaticForward | Логическое | Указывает, должно ли входящее сообщение быть автоматически пересланным, чтобы применялось условие или исключение. |
| isAutomaticReply | Логическое | Указывает, должно ли входящее сообщение быть автоматическим ответом, чтобы применялось условие или исключение. |
| isEncrypted | Логическое | Указывает, должно ли входящее сообщение быть зашифровано, чтобы применялось условие или исключение. |
| isMeetingRequest | Логическое | Указывает, должно ли входящее сообщение быть приглашением на собрание, чтобы применялось условие или исключение. |
| isMeetingResponse | Логическое | Указывает, должно ли входящее сообщение быть ответом на приглашение на собрание, чтобы применялось условие или исключение. |
| isNonDeliveryReport | Логическое | Указывает, должно ли входящее сообщение быть отчетом о недоставке, чтобы применялось условие или исключение. |
| isPermissionControlled | Логическое | Указывает, должно ли быть включено управление разрешениями (защита RMS) для входящего сообщения, чтобы к нему применялось условие или исключение. |
| isReadReceipt | Логическое | Указывает, должно ли входящее сообщение быть уведомлением о прочтении, чтобы применялось условие или исключение. |
| isSigned | Логическое | Указывает, должно ли входящее сообщение иметь подпись S/MIME, чтобы применялось условие или исключение. |
| isVoicemail | Логическое | Указывает, должно ли входящее сообщение быть сообщением голосовой почты, чтобы к нему применялось условие или исключение. |
| messageActionFlag | String  | Представляет значение флага для действия, которое должно присутствовать во входящем сообщении, чтобы к нему применялось условие или исключение. Возможные значения: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`. |
| notSentToMe | Логическое | Указывает, должно ли условие или исключение применяться только в том случае, если владелец почтового ящика не является получателем входящего сообщения. |
| recipientContains | Коллекция (String) | Представляет строки, которые должны присутствовать в свойстве **toRecipients** или **ccRecipients** входящего сообщения, чтобы к нему применялось условие или исключение. |
| senderContains | Коллекция (String) | Представляет строки, которые должны присутствовать в свойстве **from** входящего сообщения, чтобы к нему применялось условие или исключение. |
| sensitivity | String | Представляет уровень конфиденциальности, который должен быть задан для входящего сообщения, чтобы к нему применялось условие или исключение. Возможные значения: `normal`, `personal`, `private`, `confidential`. |
| sentCcMe | Логическое | Указывает, должен ли владелец почтового ящика быть указан в свойстве **ccRecipients** входящего сообщения, чтобы применялось условие или исключение. |
| sentOnlyToMe | Логическое | Указывает, должен ли владелец почтового ящика быть единственным получателем входящего сообщения, чтобы применялось условие или исключение. |
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
<!--
{
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messagerulepredicates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
