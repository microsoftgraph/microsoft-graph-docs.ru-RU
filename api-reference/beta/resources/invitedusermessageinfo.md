---
title: Настройка сообщения с приглашением
description: Объект invitedUserMessageInfo позволяет настроить сообщение с приглашением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: elisolMS
ms.openlocfilehash: 713af92d91f179f90c9d37a238a23730f351895d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989033"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="c0d2d-103">Настройка сообщения с приглашением</span><span class="sxs-lookup"><span data-stu-id="c0d2d-103">Configuring the invitation message</span></span>

<span data-ttu-id="c0d2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0d2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0d2d-105">Объект invitedUserMessageInfo позволяет настроить сообщение с [приглашением](invitation.md) .</span><span class="sxs-lookup"><span data-stu-id="c0d2d-105">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="c0d2d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0d2d-106">Properties</span></span>
| <span data-ttu-id="c0d2d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0d2d-107">Property</span></span>     | <span data-ttu-id="c0d2d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c0d2d-108">Type</span></span>   |<span data-ttu-id="c0d2d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c0d2d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0d2d-110">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="c0d2d-110">ccRecipients</span></span>|<span data-ttu-id="c0d2d-111">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="c0d2d-111">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="c0d2d-112">Дополнительные получатели сообщение о приглашении должно быть отправлено.</span><span class="sxs-lookup"><span data-stu-id="c0d2d-112">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="c0d2d-113">В настоящее время поддерживается только один дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="c0d2d-113">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="c0d2d-114">кустомизедмессажебоди</span><span class="sxs-lookup"><span data-stu-id="c0d2d-114">customizedMessageBody</span></span>|<span data-ttu-id="c0d2d-115">String</span><span class="sxs-lookup"><span data-stu-id="c0d2d-115">String</span></span>|<span data-ttu-id="c0d2d-116">Настраиваемый текст сообщения, которое вы хотите отправить, если вы не хотите использовать сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c0d2d-116">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="c0d2d-117">мессажелангуаже</span><span class="sxs-lookup"><span data-stu-id="c0d2d-117">messageLanguage</span></span>|<span data-ttu-id="c0d2d-118">String</span><span class="sxs-lookup"><span data-stu-id="c0d2d-118">String</span></span>|<span data-ttu-id="c0d2d-119">Язык, по которому необходимо отправить сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c0d2d-119">The language you want to send the default message in.</span></span> <span data-ttu-id="c0d2d-120">Если указан параметр Кустомизедмессажебоди, это свойство игнорируется, а сообщение отправляется с помощью Кустомизедмессажебоди.</span><span class="sxs-lookup"><span data-stu-id="c0d2d-120">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="c0d2d-121">Языковой формат должен быть в стандарте ISO 639.</span><span class="sxs-lookup"><span data-stu-id="c0d2d-121">The language format should be in ISO 639.</span></span> <span data-ttu-id="c0d2d-122">Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="c0d2d-122">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0d2d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0d2d-123">JSON representation</span></span>
<span data-ttu-id="c0d2d-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0d2d-124">Here is a JSON representation of the resource</span></span>

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


