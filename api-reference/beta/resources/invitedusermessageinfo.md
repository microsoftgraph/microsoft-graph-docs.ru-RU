---
title: Настройка сообщения с приглашением
description: Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f52a68cd2e6803943ac1f76fd2df12ae01f88071
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523179"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="8551e-103">Настройка сообщения с приглашением</span><span class="sxs-lookup"><span data-stu-id="8551e-103">Configuring the invitation message</span></span>

<span data-ttu-id="8551e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8551e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8551e-105">Объект invitedUserMessageInfo позволяет настроить сообщение с [приглашением](invitation.md) .</span><span class="sxs-lookup"><span data-stu-id="8551e-105">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="8551e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8551e-106">Properties</span></span>
| <span data-ttu-id="8551e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8551e-107">Property</span></span>     | <span data-ttu-id="8551e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8551e-108">Type</span></span>   |<span data-ttu-id="8551e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8551e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8551e-110">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="8551e-110">ccRecipients</span></span>|<span data-ttu-id="8551e-111">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="8551e-111">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="8551e-112">Дополнительные получатели сообщение о приглашении должно быть отправлено.</span><span class="sxs-lookup"><span data-stu-id="8551e-112">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="8551e-113">В настоящее время поддерживается только один дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="8551e-113">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="8551e-114">кустомизедмессажебоди</span><span class="sxs-lookup"><span data-stu-id="8551e-114">customizedMessageBody</span></span>|<span data-ttu-id="8551e-115">String</span><span class="sxs-lookup"><span data-stu-id="8551e-115">String</span></span>|<span data-ttu-id="8551e-116">Настраиваемый текст сообщения, которое вы хотите отправить, если вы не хотите использовать сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8551e-116">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="8551e-117">мессажелангуаже</span><span class="sxs-lookup"><span data-stu-id="8551e-117">messageLanguage</span></span>|<span data-ttu-id="8551e-118">String</span><span class="sxs-lookup"><span data-stu-id="8551e-118">String</span></span>|<span data-ttu-id="8551e-119">Язык, по которому необходимо отправить сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8551e-119">The language you want to send the default message in.</span></span> <span data-ttu-id="8551e-120">Если указан параметр Кустомизедмессажебоди, это свойство игнорируется, а сообщение отправляется с помощью Кустомизедмессажебоди.</span><span class="sxs-lookup"><span data-stu-id="8551e-120">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="8551e-121">Языковой формат должен быть в стандарте ISO 639.</span><span class="sxs-lookup"><span data-stu-id="8551e-121">The language format should be in ISO 639.</span></span> <span data-ttu-id="8551e-122">Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="8551e-122">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8551e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8551e-123">JSON representation</span></span>
<span data-ttu-id="8551e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8551e-124">Here is a JSON representation of the resource</span></span>

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
