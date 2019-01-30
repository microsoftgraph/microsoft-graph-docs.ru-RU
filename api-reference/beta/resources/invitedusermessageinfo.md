---
title: Настройка приглашения
description: Объект invitedUserMessageInfo позволяет настроить сообщение приглашение.
localization_priority: Normal
ms.openlocfilehash: fa7ead6938ddfaca78322f56f4638c45d3f2df14
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643792"
---
# <a name="configuring-the-invitation-message"></a>Настройка приглашения

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект invitedUserMessageInfo позволяет настроить сообщение [приглашение](invitation.md).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ccRecipients|[Recipients](recipient.md)|Дополнительные получатели, которым следует отправить приглашение. В настоящее время поддерживается только 1 дополнительный получатель.|
|customizedMessageBody|Строка|Ваш собственный текст сообщения, который можно отправлять вместо предоставляемого по умолчанию.|
|messageLanguage|String|Выбранный вами язык для сообщения, которое отправляется по умолчанию. Если указано значение customizedMessageBody, это свойство игнорируется, и сообщение отправляется с помощью customizedMessageBody. Язык должен быть указан в формате ISO 639. Значение по умолчанию — en-US.|

## <a name="json-representation"></a>Представление JSON
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
<!--
{
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitedusermessageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
