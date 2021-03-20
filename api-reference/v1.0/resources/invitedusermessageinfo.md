---
title: Настройка сообщения приглашения
description: Объект invitedUserMessageInfo позволяет настроить сообщение приглашения.
localization_priority: Normal
author: Sammak
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5b20eb15cfc8eb2ae248d87e5ae61ffa0d5ea08d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941381"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="d696a-103">Настройка сообщения приглашения</span><span class="sxs-lookup"><span data-stu-id="d696a-103">Configuring the invitation message</span></span>

<span data-ttu-id="d696a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d696a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d696a-105">Объект invitedUserMessageInfo позволяет настроить сообщение [приглашения.](invitation.md)</span><span class="sxs-lookup"><span data-stu-id="d696a-105">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="d696a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d696a-106">Properties</span></span>
| <span data-ttu-id="d696a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d696a-107">Property</span></span>     | <span data-ttu-id="d696a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d696a-108">Type</span></span>   |<span data-ttu-id="d696a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d696a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d696a-110">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="d696a-110">ccRecipients</span></span>|<span data-ttu-id="d696a-111">Коллекция объектов [Recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="d696a-111">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="d696a-112">Дополнительные получатели, в которые должно быть отправлено приглашение.</span><span class="sxs-lookup"><span data-stu-id="d696a-112">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="d696a-113">В настоящее время поддерживается только один дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="d696a-113">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="d696a-114">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="d696a-114">customizedMessageBody</span></span>|<span data-ttu-id="d696a-115">Строка</span><span class="sxs-lookup"><span data-stu-id="d696a-115">String</span></span>|<span data-ttu-id="d696a-116">Настраиваемый текст сообщения, который необходимо отправить, если не нужно сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d696a-116">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="d696a-117">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="d696a-117">messageLanguage</span></span>|<span data-ttu-id="d696a-118">Строка</span><span class="sxs-lookup"><span data-stu-id="d696a-118">String</span></span>|<span data-ttu-id="d696a-119">Язык, на который нужно отправить сообщение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d696a-119">The language you want to send the default message in.</span></span> <span data-ttu-id="d696a-120">Если задан настраиваемыйMessageBody, это свойство игнорируется, и сообщение отправляется с помощью настраиваемогоMessageBody.</span><span class="sxs-lookup"><span data-stu-id="d696a-120">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="d696a-121">Формат языка должен быть в ISO 639.</span><span class="sxs-lookup"><span data-stu-id="d696a-121">The language format should be in ISO 639.</span></span> <span data-ttu-id="d696a-122">По умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="d696a-122">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d696a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d696a-123">JSON representation</span></span>
<span data-ttu-id="d696a-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d696a-124">Here is a JSON representation of the resource</span></span>

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

