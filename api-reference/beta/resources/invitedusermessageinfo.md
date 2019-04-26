---
title: Настройка сообщения с приглашением
description: Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением.
localization_priority: Normal
ms.openlocfilehash: fa7ead6938ddfaca78322f56f4638c45d3f2df14
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569972"
---
# <a name="configuring-the-invitation-message"></a>Настройка сообщения с приглашением

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением [](invitation.md) .


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ccRecipients|[Получатели](recipient.md)|Дополнительные получатели сообщение о приглашении должно быть отправлено. В настоящее время поддерживается только один дополнительный получатель.|
|Кустомизедмессажебоди|String|Настраиваемый текст сообщения, которое вы хотите отправить, если вы не хотите использовать сообщение по умолчанию.|
|Мессажелангуаже|String|Язык, по которому необходимо отправить сообщение по умолчанию. Если указан параметр Кустомизедмессажебоди, это свойство игнорируется, а сообщение отправляется с помощью Кустомизедмессажебоди. Языковой формат должен быть в СТАНДАРТе ISO 639. Значение по умолчанию — en-US.|

## <a name="json-representation"></a>Описание в формате JSON
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
