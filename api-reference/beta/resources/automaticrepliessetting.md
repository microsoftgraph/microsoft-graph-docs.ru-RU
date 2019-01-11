---
title: Тип ресурса automaticRepliesSetting
description: 'Параметры конфигурации для автоматического уведомления отправителя о входящей электронной почты с сообщением '
localization_priority: Normal
ms.openlocfilehash: 0160197a4fafe10b7f78be9124da3b6260bfcee6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820659"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="847d9-103">Тип ресурса automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="847d9-103">automaticRepliesSetting resource type</span></span>

> <span data-ttu-id="847d9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="847d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="847d9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="847d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="847d9-p102">Параметры для настройки автоматического уведомления отправителя письма с помощью сообщения от пользователя, выполнившего вход. Например, для отправки автоматического ответа с уведомлением о том, что пользователь, выполнивший вход, не может отвечать на электронные сообщения.</span><span class="sxs-lookup"><span data-stu-id="847d9-p102">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="847d9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="847d9-108">Properties</span></span>
| <span data-ttu-id="847d9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="847d9-109">Property</span></span>     | <span data-ttu-id="847d9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="847d9-110">Type</span></span>   |<span data-ttu-id="847d9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="847d9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="847d9-112">externalAudience</span><span class="sxs-lookup"><span data-stu-id="847d9-112">externalAudience</span></span>|<span data-ttu-id="847d9-113">String</span><span class="sxs-lookup"><span data-stu-id="847d9-113">String</span></span>| <span data-ttu-id="847d9-p103">Внешняя аудитория по отношению к организации пользователя, выполнившего вход, которая получит сообщение **ExternalReplyMessage**, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`. Возможные значения: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="847d9-p103">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="847d9-116">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="847d9-116">externalReplyMessage</span></span>|<span data-ttu-id="847d9-117">string</span><span class="sxs-lookup"><span data-stu-id="847d9-117">string</span></span>|<span data-ttu-id="847d9-118">Автоматический ответ, который нужно отправить указанной внешней аудитории, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="847d9-118">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="847d9-119">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="847d9-119">internalReplyMessage</span></span>|<span data-ttu-id="847d9-120">string</span><span class="sxs-lookup"><span data-stu-id="847d9-120">string</span></span>|<span data-ttu-id="847d9-121">Автоматический ответ, который нужно отправить сотрудникам организации пользователя, выполнившего вход, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="847d9-121">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="847d9-122">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="847d9-122">scheduledEndDateTime</span></span>|[<span data-ttu-id="847d9-123">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="847d9-123">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="847d9-124">Дата и время завершения отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="847d9-124">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="847d9-125">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="847d9-125">scheduledStartDateTime</span></span>|[<span data-ttu-id="847d9-126">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="847d9-126">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="847d9-127">Дата и время начала отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="847d9-127">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="847d9-128">status</span><span class="sxs-lookup"><span data-stu-id="847d9-128">status</span></span>|<span data-ttu-id="847d9-129">Строка</span><span class="sxs-lookup"><span data-stu-id="847d9-129">String</span></span>|<span data-ttu-id="847d9-p104">Состояние настройки автоматических ответов. Возможные значения: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="847d9-p104">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="847d9-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="847d9-132">JSON representation</span></span>

<span data-ttu-id="847d9-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="847d9-133">Here is a JSON representation of the resource.</span></span>

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
