---
title: Тип ресурса подсказок
description: 'Информационные сообщения о получателе, отображаемых для пользователей, хотя они составлять сообщение. Например сообщение об отсутствии '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ed6d43e033b020b884a6cd1b6220b1ff566a507b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985958"
---
# <a name="mailtips-resource-type"></a>Тип ресурса подсказок

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Информационные сообщения о получателе, отображаемых для пользователей, хотя они составлять сообщение. Например отсутствии сообщение как автоматического ответа для получателя сообщения.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Почтовые подсказки для автоматического ответа, если она была настроена для получателя. |
| customMailTip | Строка | Совет настраиваемых почты, который может устанавливаться на почтовый ящик получателя. |
| deliveryRestricted| Логический | Ли почтовый ящик получателя restricted, например, прием сообщений только в стандартном списке отправителей, отклонение сообщения из предварительно заданных списка отправителей или принимать сообщения от только проверенных. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | Адрес электронной почты для получения подсказки для получателя. |
| error | [mailTipsError](../resources/mailtipserror.md) | Ошибки, возникающие во время действия [getMailTips](../api/user-getmailtips.md) . |
| externalMemberCount | Int32 | Число внешних участников, если получатель является списком рассылки. |
| isModerated |Логический  | Отправка сообщений получателю, требуется ли утверждение. Например если получатель является большой список рассылки и модератор установлен до утверждать сообщений, отправленных в этот список рассылки, или если отправка сообщений получателя требует утверждения руководителем получателя. |
| mailboxFull | Логический | Состояние полный почтовый ящик получателя. |
| maxMessageSize | Int32 | Максимальный размер сообщения, настроенного для организации или почтовый ящик получателя. |
| recipientScope | Строка | Область получателя. Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`. Например администратор может установить другой организации, чтобы быть «партнер». Область полезен в том случае, если администратор хочет определенных подсказки необходимо сделать доступным для определенных областей. Также полезно для отправителей, информирующее о том, что сообщение может привести к организации, помогая им подкорректировать формулировки, тонового сигнала и контент.|
| recipientSuggestions | Коллекция [recipient](../resources/recipient.md) | Получатели предложенных на основе предыдущих контекстах, где они отображаются в то же сообщение. |
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
