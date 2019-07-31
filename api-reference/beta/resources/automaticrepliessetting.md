---
title: Тип ресурса automaticRepliesSetting
description: 'Параметры конфигурации для автоматического уведомления отправителя о входящих сообщениях электронной почты с сообщением из '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3a4320a687ca47d89e04d61c659075cea7722e32
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013159"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="49f56-103">Тип ресурса automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="49f56-103">automaticRepliesSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49f56-p101">Параметры для настройки автоматического уведомления отправителя письма с помощью сообщения от пользователя, выполнившего вход. Например, для отправки автоматического ответа с уведомлением о том, что пользователь, выполнивший вход, не может отвечать на электронные сообщения.</span><span class="sxs-lookup"><span data-stu-id="49f56-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="49f56-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="49f56-106">Properties</span></span>
| <span data-ttu-id="49f56-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="49f56-107">Property</span></span>     | <span data-ttu-id="49f56-108">Тип</span><span class="sxs-lookup"><span data-stu-id="49f56-108">Type</span></span>   |<span data-ttu-id="49f56-109">Описание</span><span class="sxs-lookup"><span data-stu-id="49f56-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49f56-110">Екстерналаудиенце</span><span class="sxs-lookup"><span data-stu-id="49f56-110">externalAudience</span></span>|<span data-ttu-id="49f56-111">String</span><span class="sxs-lookup"><span data-stu-id="49f56-111">String</span></span>| <span data-ttu-id="49f56-p102">Внешняя аудитория по отношению к организации пользователя, выполнившего вход, которая получит сообщение **ExternalReplyMessage**, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`. Возможные значения: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="49f56-p102">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="49f56-114">Екстерналреплимессаже</span><span class="sxs-lookup"><span data-stu-id="49f56-114">externalReplyMessage</span></span>|<span data-ttu-id="49f56-115">string</span><span class="sxs-lookup"><span data-stu-id="49f56-115">string</span></span>|<span data-ttu-id="49f56-116">Автоматический ответ, который нужно отправить указанной внешней аудитории, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="49f56-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="49f56-117">Интерналреплимессаже</span><span class="sxs-lookup"><span data-stu-id="49f56-117">internalReplyMessage</span></span>|<span data-ttu-id="49f56-118">string</span><span class="sxs-lookup"><span data-stu-id="49f56-118">string</span></span>|<span data-ttu-id="49f56-119">Автоматический ответ, который нужно отправить сотрудникам организации пользователя, выполнившего вход, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="49f56-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="49f56-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="49f56-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="49f56-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="49f56-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="49f56-122">Дата и время завершения отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="49f56-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="49f56-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="49f56-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="49f56-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="49f56-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="49f56-125">Дата и время начала отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="49f56-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="49f56-126">status</span><span class="sxs-lookup"><span data-stu-id="49f56-126">status</span></span>|<span data-ttu-id="49f56-127">String</span><span class="sxs-lookup"><span data-stu-id="49f56-127">String</span></span>|<span data-ttu-id="49f56-p103">Состояние настройки автоматических ответов. Возможные значения: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="49f56-p103">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49f56-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49f56-130">JSON representation</span></span>

<span data-ttu-id="49f56-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49f56-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
