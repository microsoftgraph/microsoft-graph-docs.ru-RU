---
title: Тип ресурса mailTips
description: 'Информационные сообщения о получателе, которые отображаются пользователям во время их составления сообщения. Например, сообщение об простое '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3c72e7a81e06b267f4a212e3d56ae8607866eed2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131535"
---
# <a name="mailtips-resource-type"></a>Тип ресурса mailTips

Пространство имен: microsoft.graph

Информационные сообщения о получателе, которые отображаются пользователям во время их составления сообщения. Например, сообщение об неавтоматической службе в качестве автоматического ответа для получателя сообщения.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Подсказки электронной почты для автоматического ответа, если он был настроен получателем. |
| customMailTip | String | Пользовательская подсказка, которую можно настроить в почтовом ящике получателя. |
| deliveryRestricted| Boolean | Ограничен ли почтовый ящик получателя, например принимать сообщения только из предварительно заранее задав их или принимать сообщения только от отправителей, подлинность и т. д. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | Адрес электронной почты получателя, для который необходимо получить электронные сообщения. |
| error | [mailTipsError](../resources/mailtipserror.md) | Ошибки, которые возникают во время [действия getMailTips.](../api/user-getmailtips.md) |
| externalMemberCount | Int32 | Количество внешних членов, если получатель является списком рассылки. |
| isModerated |Boolean  | Требуется ли утверждение при отправке сообщений получателю. Например, если получатель является большим списком рассылки и модератор настроен на утверждение сообщений, отправляемых в этот список рассылки, или если для отправки сообщений получателю требуется утверждение руководителя получателя. |
| mailboxFull | Boolean | Полное состояние почтового ящика получателя. |
| maxMessageSize | Int32 | Максимальный размер сообщения, настроенный для организации или почтового ящика получателя. |
| recipientScope | recipientScopeType | Область получателя. Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`. Например, администратор может сделать другую организацию ее "партнером". Область полезна, если администратор хочет, чтобы определенные почтовые советы были доступны для определенных областей. Кроме того, отправителям полезно сообщить им о том, что их сообщения могут покинуть организацию, помогая принимать правильные решения о формулировках, тонах и содержимом.|
| recipientSuggestions | Коллекция [recipient](../resources/recipient.md) | Получатели, предлагаемые на основе предыдущих контекстов, в которых они отображаются в одном сообщении. |
| totalMemberCount | Int32 | Количество членов, если получатель является списком рассылки. |

### <a name="recipientscopetype-values"></a>Значения recipientScopeType

| Значение
|:-------------------------
| Нет
| internal
| external
| externalPartner
| externalNonPartner


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

