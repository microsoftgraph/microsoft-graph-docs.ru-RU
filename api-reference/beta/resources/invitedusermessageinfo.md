---
title: Настройка приглашения
description: Объект invitedUserMessageInfo позволяет настроить сообщение приглашение.
localization_priority: Normal
ms.openlocfilehash: f8a6dd118f1774320e3fe8327d284dac1141fc55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874125"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="1718c-103">Настройка приглашения</span><span class="sxs-lookup"><span data-stu-id="1718c-103">Configuring the invitation message</span></span>

> <span data-ttu-id="1718c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1718c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1718c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1718c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1718c-106">Объект invitedUserMessageInfo позволяет настроить сообщение [приглашение](invitation.md).</span><span class="sxs-lookup"><span data-stu-id="1718c-106">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="1718c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1718c-107">Properties</span></span>
| <span data-ttu-id="1718c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1718c-108">Property</span></span>     | <span data-ttu-id="1718c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1718c-109">Type</span></span>   |<span data-ttu-id="1718c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1718c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1718c-111">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="1718c-111">ccRecipients</span></span>|[<span data-ttu-id="1718c-112">Recipients</span><span class="sxs-lookup"><span data-stu-id="1718c-112">Recipients</span></span>](recipient.md)|<span data-ttu-id="1718c-p102">Дополнительные получатели, которым следует отправить приглашение. В настоящее время поддерживается только 1 дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="1718c-p102">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="1718c-115">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="1718c-115">customizedMessageBody</span></span>|<span data-ttu-id="1718c-116">Строка</span><span class="sxs-lookup"><span data-stu-id="1718c-116">String</span></span>|<span data-ttu-id="1718c-117">Ваш собственный текст сообщения, который можно отправлять вместо предоставляемого по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1718c-117">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="1718c-118">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="1718c-118">messageLanguage</span></span>|<span data-ttu-id="1718c-119">Строка</span><span class="sxs-lookup"><span data-stu-id="1718c-119">String</span></span>|<span data-ttu-id="1718c-p103">Выбранный вами язык для сообщения, которое отправляется по умолчанию. Если указано значение customizedMessageBody, это свойство игнорируется, и сообщение отправляется с помощью customizedMessageBody. Язык должен быть указан в формате ISO 639. Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="1718c-p103">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1718c-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1718c-124">JSON representation</span></span>
<span data-ttu-id="1718c-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1718c-125">Here is a JSON representation of the resource</span></span>

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
