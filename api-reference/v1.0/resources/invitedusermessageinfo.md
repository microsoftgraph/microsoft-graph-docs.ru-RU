---
title: Настройка сообщения приглашения
description: Объект invitedUserMessageInfo позволяет настроить сообщение приглашения.
localization_priority: Normal
author: elisolMS
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d44542b26fd1c1ffb7b70dcfc019ada6f0cc02f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129725"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="9e355-103">Настройка сообщения приглашения</span><span class="sxs-lookup"><span data-stu-id="9e355-103">Configuring the invitation message</span></span>

<span data-ttu-id="9e355-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e355-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e355-105">Объект invitedUserMessageInfo позволяет настроить сообщение [приглашения.](invitation.md)</span><span class="sxs-lookup"><span data-stu-id="9e355-105">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="9e355-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e355-106">Properties</span></span>
| <span data-ttu-id="9e355-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e355-107">Property</span></span>     | <span data-ttu-id="9e355-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9e355-108">Type</span></span>   |<span data-ttu-id="9e355-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9e355-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e355-110">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="9e355-110">ccRecipients</span></span>|<span data-ttu-id="9e355-111">Коллекция объектов [Recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="9e355-111">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="9e355-112">Дополнительные получатели, на которые должно быть отправлено приглашение.</span><span class="sxs-lookup"><span data-stu-id="9e355-112">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="9e355-113">В настоящее время поддерживается только один дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="9e355-113">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="9e355-114">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="9e355-114">customizedMessageBody</span></span>|<span data-ttu-id="9e355-115">String</span><span class="sxs-lookup"><span data-stu-id="9e355-115">String</span></span>|<span data-ttu-id="9e355-116">Настраиваемый текст сообщения, который необходимо отправить, если сообщение по умолчанию не нужно.</span><span class="sxs-lookup"><span data-stu-id="9e355-116">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="9e355-117">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="9e355-117">messageLanguage</span></span>|<span data-ttu-id="9e355-118">String</span><span class="sxs-lookup"><span data-stu-id="9e355-118">String</span></span>|<span data-ttu-id="9e355-119">Язык, на который вы хотите отправить сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9e355-119">The language you want to send the default message in.</span></span> <span data-ttu-id="9e355-120">Если задан параметр customizedMessageBody, это свойство игнорируется, и сообщение отправляется с помощью параметра customizedMessageBody.</span><span class="sxs-lookup"><span data-stu-id="9e355-120">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="9e355-121">Формат языка должен быть в формате ISO 639.</span><span class="sxs-lookup"><span data-stu-id="9e355-121">The language format should be in ISO 639.</span></span> <span data-ttu-id="9e355-122">Значение по умолчанию : en-US.</span><span class="sxs-lookup"><span data-stu-id="9e355-122">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e355-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e355-123">JSON representation</span></span>
<span data-ttu-id="9e355-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e355-124">Here is a JSON representation of the resource</span></span>

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

