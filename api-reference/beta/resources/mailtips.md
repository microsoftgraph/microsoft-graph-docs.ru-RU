---
title: Тип ресурса подсказок
description: 'Информационные сообщения о получателе, отображаемых для пользователей, хотя они составлять сообщение. Например сообщение об отсутствии '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11e64c09a90d130b7656d4e87770e6df3fb67408
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508414"
---
# <a name="mailtips-resource-type"></a>Тип ресурса подсказок

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Информационные сообщения о получателе, отображаемых для пользователей, хотя они составлять сообщение. Например отсутствии сообщение как автоматического ответа для получателя сообщения.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Почтовые подсказки для автоматического ответа, если она была настроена для получателя. |
| CustomMailTip | String | Совет настраиваемых почты, который может устанавливаться на почтовый ящик получателя. |
| DeliveryRestricted| Логическое | Ли почтовый ящик получателя restricted, например, прием сообщений только в стандартном списке отправителей, отклонение сообщения из предварительно заданных списка отправителей или принимать сообщения от только проверенных. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | Адрес электронной почты для получения подсказки для получателя. |
| error | [mailTipsError](../resources/mailtipserror.md) | Ошибки, возникающие во время действия [getMailTips](../api/user-getmailtips.md) . |
| ExternalMemberCount | Int32 | Число внешних участников, если получатель является списком рассылки. |
| IsModerated |Логическое  | Отправка сообщений получателю, требуется ли утверждение. Например если получатель является большой список рассылки и модератор установлен до утверждать сообщений, отправленных в этот список рассылки, или если отправка сообщений получателя требует утверждения руководителем получателя. |
| MailboxFull | Логическое | Состояние полный почтовый ящик получателя. |
| MaxMessageSize | Int32 | Максимальный размер сообщения, настроенного для организации или почтовый ящик получателя. |
| recipientScope | String | Область получателя. Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`. Например администратор может установить другой организации, чтобы быть «партнер». Область полезен в том случае, если администратор хочет определенных подсказки необходимо сделать доступным для определенных областей. Также полезно для отправителей, информирующее о том, что сообщение может привести к организации, помогая им подкорректировать формулировки, тонового сигнала и контент.|
| recipientSuggestions | Коллекция [recipient](../resources/recipient.md) | Получатели предложенных на основе предыдущих контекстах, где они отображаются в то же сообщение. |
| TotalMemberCount | Int32 | Число участников, если получатель является списком рассылки. |

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
<!--
{
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
