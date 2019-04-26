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
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="a0167-103">Настройка сообщения с приглашением</span><span class="sxs-lookup"><span data-stu-id="a0167-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0167-104">Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением [](invitation.md) .</span><span class="sxs-lookup"><span data-stu-id="a0167-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="a0167-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0167-105">Properties</span></span>
| <span data-ttu-id="a0167-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0167-106">Property</span></span>     | <span data-ttu-id="a0167-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a0167-107">Type</span></span>   |<span data-ttu-id="a0167-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a0167-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0167-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="a0167-109">ccRecipients</span></span>|[<span data-ttu-id="a0167-110">Получатели</span><span class="sxs-lookup"><span data-stu-id="a0167-110">Recipients</span></span>](recipient.md)|<span data-ttu-id="a0167-111">Дополнительные получатели сообщение о приглашении должно быть отправлено.</span><span class="sxs-lookup"><span data-stu-id="a0167-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="a0167-112">В настоящее время поддерживается только один дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="a0167-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="a0167-113">Кустомизедмессажебоди</span><span class="sxs-lookup"><span data-stu-id="a0167-113">customizedMessageBody</span></span>|<span data-ttu-id="a0167-114">String</span><span class="sxs-lookup"><span data-stu-id="a0167-114">String</span></span>|<span data-ttu-id="a0167-115">Настраиваемый текст сообщения, которое вы хотите отправить, если вы не хотите использовать сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a0167-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="a0167-116">Мессажелангуаже</span><span class="sxs-lookup"><span data-stu-id="a0167-116">messageLanguage</span></span>|<span data-ttu-id="a0167-117">String</span><span class="sxs-lookup"><span data-stu-id="a0167-117">String</span></span>|<span data-ttu-id="a0167-118">Язык, по которому необходимо отправить сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a0167-118">The language you want to send the default message in.</span></span> <span data-ttu-id="a0167-119">Если указан параметр Кустомизедмессажебоди, это свойство игнорируется, а сообщение отправляется с помощью Кустомизедмессажебоди.</span><span class="sxs-lookup"><span data-stu-id="a0167-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="a0167-120">Языковой формат должен быть в СТАНДАРТе ISO 639.</span><span class="sxs-lookup"><span data-stu-id="a0167-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="a0167-121">Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="a0167-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0167-122">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a0167-122">JSON representation</span></span>
<span data-ttu-id="a0167-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0167-123">Here is a JSON representation of the resource</span></span>

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
