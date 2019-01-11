---
title: Настройка приглашения
description: Объект invitedUserMessageInfo позволяет настроить сообщение приглашение.
localization_priority: Normal
ms.openlocfilehash: 06be157e61fd6d466cc2b18546bb29762d0133a8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885871"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="ed2b8-103">Настройка приглашения</span><span class="sxs-lookup"><span data-stu-id="ed2b8-103">Configuring the invitation message</span></span>

<span data-ttu-id="ed2b8-104">Объект invitedUserMessageInfo позволяет настроить сообщение [приглашение](invitation.md).</span><span class="sxs-lookup"><span data-stu-id="ed2b8-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="ed2b8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed2b8-105">Properties</span></span>
| <span data-ttu-id="ed2b8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed2b8-106">Property</span></span>     | <span data-ttu-id="ed2b8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ed2b8-107">Type</span></span>   |<span data-ttu-id="ed2b8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ed2b8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed2b8-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="ed2b8-109">ccRecipients</span></span>|<span data-ttu-id="ed2b8-110">Коллекция объектов [Recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="ed2b8-110">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="ed2b8-p101">Дополнительные получатели, которым следует отправить приглашение. В настоящее время поддерживается только 1 дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="ed2b8-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="ed2b8-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="ed2b8-113">customizedMessageBody</span></span>|<span data-ttu-id="ed2b8-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ed2b8-114">String</span></span>|<span data-ttu-id="ed2b8-115">Ваш собственный текст сообщения, который можно отправлять вместо предоставляемого по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ed2b8-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="ed2b8-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="ed2b8-116">messageLanguage</span></span>|<span data-ttu-id="ed2b8-117">Строка</span><span class="sxs-lookup"><span data-stu-id="ed2b8-117">String</span></span>|<span data-ttu-id="ed2b8-p102">Выбранный вами язык для сообщения, которое отправляется по умолчанию. Если указано значение customizedMessageBody, это свойство игнорируется, и сообщение отправляется с помощью customizedMessageBody. Язык должен быть указан в формате ISO 639. Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="ed2b8-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed2b8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed2b8-122">JSON representation</span></span>
<span data-ttu-id="ed2b8-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed2b8-123">Here is a JSON representation of the resource</span></span>

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
