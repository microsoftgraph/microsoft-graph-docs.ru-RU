---
title: Настройка приглашения
description: Объект invitedUserMessageInfo позволяет настроить сообщение приглашение.
ms.openlocfilehash: c8258d2b90d1aa5f5081b271ccc70fcb7408b132
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027610"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="f5986-103">Настройка приглашения</span><span class="sxs-lookup"><span data-stu-id="f5986-103">Configuring the invitation message</span></span>

<span data-ttu-id="f5986-104">Объект invitedUserMessageInfo позволяет настроить сообщение [приглашение](invitation.md).</span><span class="sxs-lookup"><span data-stu-id="f5986-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="f5986-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5986-105">Properties</span></span>
| <span data-ttu-id="f5986-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5986-106">Property</span></span>     | <span data-ttu-id="f5986-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f5986-107">Type</span></span>   |<span data-ttu-id="f5986-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f5986-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5986-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="f5986-109">ccRecipients</span></span>|<span data-ttu-id="f5986-110">Коллекция объектов [Recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f5986-110">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="f5986-p101">Дополнительные получатели, которым следует отправить приглашение. В настоящее время поддерживается только 1 дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="f5986-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="f5986-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="f5986-113">customizedMessageBody</span></span>|<span data-ttu-id="f5986-114">Строка</span><span class="sxs-lookup"><span data-stu-id="f5986-114">String</span></span>|<span data-ttu-id="f5986-115">Ваш собственный текст сообщения, который можно отправлять вместо предоставляемого по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f5986-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="f5986-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="f5986-116">messageLanguage</span></span>|<span data-ttu-id="f5986-117">String</span><span class="sxs-lookup"><span data-stu-id="f5986-117">String</span></span>|<span data-ttu-id="f5986-p102">Выбранный вами язык для сообщения, которое отправляется по умолчанию. Если указано значение customizedMessageBody, это свойство игнорируется, и сообщение отправляется с помощью customizedMessageBody. Язык должен быть указан в формате ISO 639. Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="f5986-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5986-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5986-122">JSON representation</span></span>
<span data-ttu-id="f5986-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5986-123">Here is a JSON representation of the resource</span></span>

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
