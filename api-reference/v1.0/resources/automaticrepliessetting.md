---
title: Тип ресурса automaticRepliesSetting
description: 'Параметры конфигурации для автоматического уведомления отправителя о входящей электронной почты с сообщением '
localization_priority: Normal
ms.openlocfilehash: 81fb16a9124c60f43887150917f132579aa4f163
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821408"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="b966e-103">Тип ресурса automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b966e-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="b966e-p101">Параметры для настройки автоматического уведомления отправителя письма с помощью сообщения от пользователя, выполнившего вход. Например, для отправки автоматического ответа с уведомлением о том, что пользователь, выполнивший вход, не может отвечать на электронные сообщения.</span><span class="sxs-lookup"><span data-stu-id="b966e-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="b966e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b966e-106">Properties</span></span>
| <span data-ttu-id="b966e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b966e-107">Property</span></span>     | <span data-ttu-id="b966e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b966e-108">Type</span></span>   |<span data-ttu-id="b966e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b966e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b966e-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="b966e-110">externalAudience</span></span>|<span data-ttu-id="b966e-111">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="b966e-111">externalAudienceScope</span></span>| <span data-ttu-id="b966e-112">Набор аудитории, внешними по отношению к организации пользователь выполнил вход пользователей, которые будут иметь **ExternalReplyMessage**, если **состояние** `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b966e-112">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> <span data-ttu-id="b966e-113">Возможные значения: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="b966e-113">The possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="b966e-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="b966e-114">externalReplyMessage</span></span>|<span data-ttu-id="b966e-115">string</span><span class="sxs-lookup"><span data-stu-id="b966e-115">string</span></span>|<span data-ttu-id="b966e-116">Автоматический ответ, который нужно отправить указанной внешней аудитории, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b966e-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="b966e-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="b966e-117">internalReplyMessage</span></span>|<span data-ttu-id="b966e-118">string</span><span class="sxs-lookup"><span data-stu-id="b966e-118">string</span></span>|<span data-ttu-id="b966e-119">Автоматический ответ, который нужно отправить сотрудникам организации пользователя, выполнившего вход, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b966e-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="b966e-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="b966e-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="b966e-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b966e-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b966e-122">Дата и время завершения отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b966e-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="b966e-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="b966e-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="b966e-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b966e-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b966e-125">Дата и время начала отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b966e-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="b966e-126">status</span><span class="sxs-lookup"><span data-stu-id="b966e-126">status</span></span>|<span data-ttu-id="b966e-127">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="b966e-127">automaticRepliesStatus</span></span>|<span data-ttu-id="b966e-128">Состояние конфигурации для автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="b966e-128">Configurations status for automatic replies.</span></span> <span data-ttu-id="b966e-129">Возможные значения: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="b966e-129">The possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b966e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b966e-130">JSON representation</span></span>

<span data-ttu-id="b966e-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b966e-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
