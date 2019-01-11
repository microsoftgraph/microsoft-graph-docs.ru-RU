---
title: Тип ресурса workingHours
description: Представляет дни недели и часы работы пользователя в определенном часовом поясе.
localization_priority: Normal
ms.openlocfilehash: d34da38ad1a007f6c63154cb496006585df95c13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885742"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="c040f-103">Тип ресурса workingHours</span><span class="sxs-lookup"><span data-stu-id="c040f-103">workingHours resource type</span></span>

> <span data-ttu-id="c040f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c040f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c040f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c040f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c040f-106">Представляет дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="c040f-106">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="c040f-107">Доступ к рабочему времени пользователя полезен в тех случаях, когда требуется планировать действия или ресурсы.</span><span class="sxs-lookup"><span data-stu-id="c040f-107">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="c040f-108">Вы можете [получать](../api/user-get-mailboxsettings.md#request-3) и [задавать](../api/user-update-mailboxsettings.md#request-2) рабочее время пользователя в [параметрах его почтового ящика](mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="c040f-108">You can [get](../api/user-get-mailboxsettings.md#request-3) and [set](../api/user-update-mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="c040f-109">Вы можете задать часовой пояс для своего рабочего времени отдельно от часового пояса, заданного для клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="c040f-109">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="c040f-110">Например, это может быть полезно, если вы перемещаетесь в другой часовой пояс, где вы обычно не работаете.</span><span class="sxs-lookup"><span data-stu-id="c040f-110">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="c040f-111">Для клиента Outlook</span><span class="sxs-lookup"><span data-stu-id="c040f-111">You can set the Outlook client</span></span>  
<span data-ttu-id="c040f-112">можно задать целевой часовой пояс, чтобы значения времени в Outlook соответствовали местному времени, пока вы там находитесь.</span><span class="sxs-lookup"><span data-stu-id="c040f-112">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="c040f-113">Когда другие люди запрашивают рабочие встречи с вами на вашем обычном рабочем месте, они по-прежнему могут учитывать ваше рабочее время в соответствующем часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="c040f-113">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="c040f-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="c040f-114">Properties</span></span>
| <span data-ttu-id="c040f-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="c040f-115">Property</span></span>     | <span data-ttu-id="c040f-116">Тип</span><span class="sxs-lookup"><span data-stu-id="c040f-116">Type</span></span>   |<span data-ttu-id="c040f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c040f-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c040f-118">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="c040f-118">daysOfWeek</span></span> | <span data-ttu-id="c040f-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c040f-119">String collection</span></span> | <span data-ttu-id="c040f-120">Дни недели, в которые работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="c040f-120">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="c040f-121">startTime</span><span class="sxs-lookup"><span data-stu-id="c040f-121">startTime</span></span> | <span data-ttu-id="c040f-122">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c040f-122">Edm.TimeOfDay</span></span> | <span data-ttu-id="c040f-123">Время дня, в которое пользователь начинает работать.</span><span class="sxs-lookup"><span data-stu-id="c040f-123">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="c040f-124">endTime</span><span class="sxs-lookup"><span data-stu-id="c040f-124">endTime</span></span> | <span data-ttu-id="c040f-125">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c040f-125">Edm.TimeOfDay</span></span> | <span data-ttu-id="c040f-126">Время дня, в которое пользователь заканчивает работать.</span><span class="sxs-lookup"><span data-stu-id="c040f-126">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="c040f-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="c040f-127">timeZone</span></span> | [<span data-ttu-id="c040f-128">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="c040f-128">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="c040f-129">Часовой пояс, к которому относится рабочее время.</span><span class="sxs-lookup"><span data-stu-id="c040f-129">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c040f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c040f-130">JSON representation</span></span>

<span data-ttu-id="c040f-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c040f-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
