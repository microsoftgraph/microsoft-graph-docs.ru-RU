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
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="77c41-103">Настройка приглашения</span><span class="sxs-lookup"><span data-stu-id="77c41-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77c41-104">Объект invitedUserMessageInfo позволяет настроить сообщение [приглашение](invitation.md).</span><span class="sxs-lookup"><span data-stu-id="77c41-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="77c41-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="77c41-105">Properties</span></span>
| <span data-ttu-id="77c41-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="77c41-106">Property</span></span>     | <span data-ttu-id="77c41-107">Тип</span><span class="sxs-lookup"><span data-stu-id="77c41-107">Type</span></span>   |<span data-ttu-id="77c41-108">Описание</span><span class="sxs-lookup"><span data-stu-id="77c41-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77c41-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="77c41-109">ccRecipients</span></span>|[<span data-ttu-id="77c41-110">Recipients</span><span class="sxs-lookup"><span data-stu-id="77c41-110">Recipients</span></span>](recipient.md)|<span data-ttu-id="77c41-p101">Дополнительные получатели, которым следует отправить приглашение. В настоящее время поддерживается только 1 дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="77c41-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="77c41-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="77c41-113">customizedMessageBody</span></span>|<span data-ttu-id="77c41-114">Строка</span><span class="sxs-lookup"><span data-stu-id="77c41-114">String</span></span>|<span data-ttu-id="77c41-115">Ваш собственный текст сообщения, который можно отправлять вместо предоставляемого по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="77c41-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="77c41-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="77c41-116">messageLanguage</span></span>|<span data-ttu-id="77c41-117">String</span><span class="sxs-lookup"><span data-stu-id="77c41-117">String</span></span>|<span data-ttu-id="77c41-p102">Выбранный вами язык для сообщения, которое отправляется по умолчанию. Если указано значение customizedMessageBody, это свойство игнорируется, и сообщение отправляется с помощью customizedMessageBody. Язык должен быть указан в формате ISO 639. Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="77c41-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77c41-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77c41-122">JSON representation</span></span>
<span data-ttu-id="77c41-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77c41-123">Here is a JSON representation of the resource</span></span>

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
