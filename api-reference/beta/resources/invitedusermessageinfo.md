---
title: Настройка сообщения с приглашением
description: Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением.
localization_priority: Normal
ms.openlocfilehash: 458efdade9b5cd7b538ffa3e217ec915dac93ad9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341353"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="60d90-103">Настройка сообщения с приглашением</span><span class="sxs-lookup"><span data-stu-id="60d90-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60d90-104">Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением [](invitation.md) .</span><span class="sxs-lookup"><span data-stu-id="60d90-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="60d90-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="60d90-105">Properties</span></span>
| <span data-ttu-id="60d90-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="60d90-106">Property</span></span>     | <span data-ttu-id="60d90-107">Тип</span><span class="sxs-lookup"><span data-stu-id="60d90-107">Type</span></span>   |<span data-ttu-id="60d90-108">Описание</span><span class="sxs-lookup"><span data-stu-id="60d90-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60d90-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="60d90-109">ccRecipients</span></span>|<span data-ttu-id="60d90-110">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="60d90-110">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="60d90-111">Дополнительные получатели сообщение о приглашении должно быть отправлено.</span><span class="sxs-lookup"><span data-stu-id="60d90-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="60d90-112">В настоящее время поддерживается только один дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="60d90-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="60d90-113">Кустомизедмессажебоди</span><span class="sxs-lookup"><span data-stu-id="60d90-113">customizedMessageBody</span></span>|<span data-ttu-id="60d90-114">String</span><span class="sxs-lookup"><span data-stu-id="60d90-114">String</span></span>|<span data-ttu-id="60d90-115">Настраиваемый текст сообщения, которое вы хотите отправить, если вы не хотите использовать сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="60d90-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="60d90-116">Мессажелангуаже</span><span class="sxs-lookup"><span data-stu-id="60d90-116">messageLanguage</span></span>|<span data-ttu-id="60d90-117">String</span><span class="sxs-lookup"><span data-stu-id="60d90-117">String</span></span>|<span data-ttu-id="60d90-118">Язык, по которому необходимо отправить сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="60d90-118">The language you want to send the default message in.</span></span> <span data-ttu-id="60d90-119">Если указан параметр Кустомизедмессажебоди, это свойство игнорируется, а сообщение отправляется с помощью Кустомизедмессажебоди.</span><span class="sxs-lookup"><span data-stu-id="60d90-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="60d90-120">Языковой формат должен быть в СТАНДАРТе ISO 639.</span><span class="sxs-lookup"><span data-stu-id="60d90-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="60d90-121">Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="60d90-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60d90-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60d90-122">JSON representation</span></span>
<span data-ttu-id="60d90-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60d90-123">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
