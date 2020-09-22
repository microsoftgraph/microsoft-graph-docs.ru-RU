---
title: Тип ресурса подсказки
description: 'Информативные сообщения о получателе, которые отображаются для пользователей во время составления сообщения. Например, сообщение об отсутствии на работе '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 337d280df51d86aadb879b01fa5bfa5bf4e77e9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021429"
---
# <a name="mailtips-resource-type"></a>Тип ресурса подсказки

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Информативные сообщения о получателе, которые отображаются для пользователей во время составления сообщения. Например, сообщение об отсутствии на работе в качестве автоматического ответа для получателя сообщения.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| аутоматикреплиес | [аутоматикреплиесмаилтипс](../resources/automaticrepliesmailtips.md) | Советы по использованию электронной почты для автоматического ответа, если он настроен получателем. |
| кустоммаилтип | String | Настраиваемая подсказка почты, которую можно настроить для почтового ящика получателя. |
| деливерирестриктед| Boolean | Является ли почтовый ящик получателя ограниченным, например принимать сообщения только от предопределенного списка отправителей, отклонять сообщения из предопределенного списка отправителей или принимать сообщения только от отправителей, прошедших проверку подлинности. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | Адрес электронной почты получателя, для которого необходимо получить подсказки. |
| error | [маилтипсеррор](../resources/mailtipserror.md) | Ошибки, возникающие при выполнении действия [подсказки](../api/user-getmailtips.md) . |
| екстерналмемберкаунт | Int32 | Количество внешних участников, если получатель является списком рассылки. |
| Модератор |Boolean  | Требуется ли утверждение для отправки сообщений получателю. Например, если получатель является большим списком рассылки, а Модератор настроен на утверждение сообщений, отправленных в этот список рассылки, или если отправка сообщений получателю требует утверждения руководителя получателя. |
| маилбоксфулл | Boolean | Полный статус почтового ящика получателя. |
| maxMessageSize | Int32 | Максимальный размер сообщения, настроенный для организации или почтового ящика получателя. |
| реЦипиентскопе | String | Область получателя. Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`. Например, администратор может назначить другую организацию "партнером". Область действия полезна, если администратору требуется, чтобы некоторые подсказки были доступны для определенных областей. Кроме того, отправители могут уведомить пользователей о том, что их сообщения могут отказаться от Организации, помогая им принять правильные решения по работе со словами, тонами и содержимым.|
| реЦипиентсугжестионс | Коллекция [recipient](../resources/recipient.md) | Получатели, предлагаемые в соответствии с предыдущими контекстами, в которых они отображаются в одном сообщении. |
| тоталмемберкаунт | Int32 | Число участников, если получатель является списком рассылки. |

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
  "suppressions": []
}
-->


