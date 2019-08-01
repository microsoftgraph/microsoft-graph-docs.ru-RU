---
title: Настройка сообщения с приглашением
description: Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fff33ce5ceda9ea3c60583338538a1bf502ae0f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036752"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="271c6-103">Настройка сообщения с приглашением</span><span class="sxs-lookup"><span data-stu-id="271c6-103">Configuring the invitation message</span></span>

<span data-ttu-id="271c6-104">Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением [](invitation.md) .</span><span class="sxs-lookup"><span data-stu-id="271c6-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="271c6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="271c6-105">Properties</span></span>
| <span data-ttu-id="271c6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="271c6-106">Property</span></span>     | <span data-ttu-id="271c6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="271c6-107">Type</span></span>   |<span data-ttu-id="271c6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="271c6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="271c6-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="271c6-109">ccRecipients</span></span>|<span data-ttu-id="271c6-110">Коллекция объектов [Recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="271c6-110">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="271c6-111">Дополнительные получатели сообщение о приглашении должно быть отправлено.</span><span class="sxs-lookup"><span data-stu-id="271c6-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="271c6-112">В настоящее время поддерживается только один дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="271c6-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="271c6-113">Кустомизедмессажебоди</span><span class="sxs-lookup"><span data-stu-id="271c6-113">customizedMessageBody</span></span>|<span data-ttu-id="271c6-114">String</span><span class="sxs-lookup"><span data-stu-id="271c6-114">String</span></span>|<span data-ttu-id="271c6-115">Настраиваемый текст сообщения, которое вы хотите отправить, если вы не хотите использовать сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="271c6-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="271c6-116">Мессажелангуаже</span><span class="sxs-lookup"><span data-stu-id="271c6-116">messageLanguage</span></span>|<span data-ttu-id="271c6-117">String</span><span class="sxs-lookup"><span data-stu-id="271c6-117">String</span></span>|<span data-ttu-id="271c6-118">Язык, по которому необходимо отправить сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="271c6-118">The language you want to send the default message in.</span></span> <span data-ttu-id="271c6-119">Если указан параметр Кустомизедмессажебоди, это свойство игнорируется, а сообщение отправляется с помощью Кустомизедмессажебоди.</span><span class="sxs-lookup"><span data-stu-id="271c6-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="271c6-120">Языковой формат должен быть в стандарте ISO 639.</span><span class="sxs-lookup"><span data-stu-id="271c6-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="271c6-121">Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="271c6-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="271c6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="271c6-122">JSON representation</span></span>
<span data-ttu-id="271c6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="271c6-123">Here is a JSON representation of the resource</span></span>

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
