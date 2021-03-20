---
title: тип ресурса mailTips
description: 'Информативные сообщения о получателе, отображаемые пользователям во время их составления сообщения. Например, неавтное сообщение '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0a2dfe421c19b49c8c7f489bef55890a058e2c40
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941374"
---
# <a name="mailtips-resource-type"></a>тип ресурса mailTips

Пространство имен: microsoft.graph

Информативные сообщения о получателе, отображаемые пользователям во время их составления сообщения. Например, неавтоматическое сообщение в качестве автоматического ответа для получателя сообщения.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Советы по электронной почте для автоматического ответа, если оно было настроено получателем. |
| customMailTip | Строка | Пользовательский совет по почте, который можно установить на почтовом ящике получателя. |
| deliveryRestricted| Boolean | Ограничен ли почтовый ящик получателя, например, прием сообщений только из предварительного списка отправителей, отклонение сообщений из предварительного списка отправителей или прием сообщений только от авторов проверки подлинности. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | Адрес электронной почты получателя для получения почтовых отправлений. |
| error | [mailTipsError](../resources/mailtipserror.md) | Ошибки, которые возникают во время [действия getMailTips.](../api/user-getmailtips.md) |
| externalMemberCount | Int32 | Количество внешних участников, если получатель — это список рассылки. |
| isModerated |Boolean  | Требуется ли для отправки сообщений получателю утверждение. Например, если получатель — это большой список рассылки и модератор настроен для утверждения сообщений, отправленных в этот список рассылки, или если отправка сообщений получателю требует утверждения руководителя получателя. |
| mailboxFull | Boolean | Полный статус почтового ящика получателя. |
| maxMessageSize | Int32 | Максимальный размер сообщения, настроенный для организации или почтового ящика получателя. |
| recipientScope | recipientScopeType | Область получателя. Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`. Например, администратор может установить, что другая организация является ее "партнером". Область полезна, если администратор хочет, чтобы определенные почтовые ящики были доступны для определенных областей. Кроме того, отправителям полезно информировать их о том, что их сообщение может покинуть организацию, помогая им принимать правильные решения о формулировках, тоне и контенте.|
| recipientSuggestions | Коллекция [recipient](../resources/recipient.md) | Получатели предлагаются на основе предыдущих контекстов, в которых они отображаются в одном сообщении. |
| totalMemberCount | Int32 | Количество участников, если получатель — это список рассылки. |

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

