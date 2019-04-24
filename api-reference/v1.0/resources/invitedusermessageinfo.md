---
title: Настройка сообщения с приглашением
description: Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением.
localization_priority: Normal
ms.openlocfilehash: 06be157e61fd6d466cc2b18546bb29762d0133a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585120"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="46308-103">Настройка сообщения с приглашением</span><span class="sxs-lookup"><span data-stu-id="46308-103">Configuring the invitation message</span></span>

<span data-ttu-id="46308-104">Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением [](invitation.md) .</span><span class="sxs-lookup"><span data-stu-id="46308-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="46308-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="46308-105">Properties</span></span>
| <span data-ttu-id="46308-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="46308-106">Property</span></span>     | <span data-ttu-id="46308-107">Тип</span><span class="sxs-lookup"><span data-stu-id="46308-107">Type</span></span>   |<span data-ttu-id="46308-108">Описание</span><span class="sxs-lookup"><span data-stu-id="46308-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46308-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="46308-109">ccRecipients</span></span>|<span data-ttu-id="46308-110">Коллекция объектов [Recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="46308-110">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="46308-111">Дополнительные получатели сообщение о приглашении должно быть отправлено.</span><span class="sxs-lookup"><span data-stu-id="46308-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="46308-112">В настоящее время поддерживается только один дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="46308-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="46308-113">Кустомизедмессажебоди</span><span class="sxs-lookup"><span data-stu-id="46308-113">customizedMessageBody</span></span>|<span data-ttu-id="46308-114">String</span><span class="sxs-lookup"><span data-stu-id="46308-114">String</span></span>|<span data-ttu-id="46308-115">Настраиваемый текст сообщения, которое вы хотите отправить, если вы не хотите использовать сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="46308-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="46308-116">Мессажелангуаже</span><span class="sxs-lookup"><span data-stu-id="46308-116">messageLanguage</span></span>|<span data-ttu-id="46308-117">String</span><span class="sxs-lookup"><span data-stu-id="46308-117">String</span></span>|<span data-ttu-id="46308-118">Язык, по которому необходимо отправить сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="46308-118">The language you want to send the default message in.</span></span> <span data-ttu-id="46308-119">Если указан параметр Кустомизедмессажебоди, это свойство игнорируется, а сообщение отправляется с помощью Кустомизедмессажебоди.</span><span class="sxs-lookup"><span data-stu-id="46308-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="46308-120">Языковой формат должен быть в СТАНДАРТе ISO 639.</span><span class="sxs-lookup"><span data-stu-id="46308-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="46308-121">Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="46308-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46308-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46308-122">JSON representation</span></span>
<span data-ttu-id="46308-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46308-123">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
