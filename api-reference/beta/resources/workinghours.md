---
title: Тип ресурса workingHours
description: Представляет дни недели и часы работы пользователя в определенном часовом поясе.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 5e86df6eae7d1ae399cb764321e8fc2af1815409
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472410"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="896c3-103">Тип ресурса workingHours</span><span class="sxs-lookup"><span data-stu-id="896c3-103">workingHours resource type</span></span>

<span data-ttu-id="896c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="896c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="896c3-105">Представляет дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="896c3-105">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="896c3-106">Доступ к рабочему времени пользователя полезен в тех случаях, когда требуется планировать действия или ресурсы.</span><span class="sxs-lookup"><span data-stu-id="896c3-106">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="896c3-107">Вы можете [получать](../api/user-get-mailboxsettings.md#example-3) и [задавать](../api/user-update-mailboxsettings.md#example-2) рабочее время пользователя в [параметрах его почтового ящика](mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="896c3-107">You can [get](../api/user-get-mailboxsettings.md#example-3) and [set](../api/user-update-mailboxsettings.md#example-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="896c3-108">Вы можете задать часовой пояс для своего рабочего времени отдельно от часового пояса, заданного для клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="896c3-108">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="896c3-109">Например, это может быть полезно, если вы перемещаетесь в другой часовой пояс, где вы обычно не работаете.</span><span class="sxs-lookup"><span data-stu-id="896c3-109">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="896c3-110">Для клиента Outlook</span><span class="sxs-lookup"><span data-stu-id="896c3-110">You can set the Outlook client</span></span>  
<span data-ttu-id="896c3-111">можно задать целевой часовой пояс, чтобы значения времени в Outlook соответствовали местному времени, пока вы там находитесь.</span><span class="sxs-lookup"><span data-stu-id="896c3-111">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="896c3-112">Когда другие люди запрашивают рабочие встречи с вами на вашем обычном рабочем месте, они по-прежнему могут учитывать ваше рабочее время в соответствующем часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="896c3-112">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="896c3-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="896c3-113">Properties</span></span>
| <span data-ttu-id="896c3-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="896c3-114">Property</span></span>     | <span data-ttu-id="896c3-115">Тип</span><span class="sxs-lookup"><span data-stu-id="896c3-115">Type</span></span>   |<span data-ttu-id="896c3-116">Описание</span><span class="sxs-lookup"><span data-stu-id="896c3-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="896c3-117">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="896c3-117">daysOfWeek</span></span> | <span data-ttu-id="896c3-118">коллекция dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="896c3-118">dayOfWeek collection</span></span> | <span data-ttu-id="896c3-119">Дни недели, в которые работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="896c3-119">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="896c3-120">startTime</span><span class="sxs-lookup"><span data-stu-id="896c3-120">startTime</span></span> | <span data-ttu-id="896c3-121">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="896c3-121">Edm.TimeOfDay</span></span> | <span data-ttu-id="896c3-122">Время дня, в которое пользователь начинает работать.</span><span class="sxs-lookup"><span data-stu-id="896c3-122">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="896c3-123">endTime</span><span class="sxs-lookup"><span data-stu-id="896c3-123">endTime</span></span> | <span data-ttu-id="896c3-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="896c3-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="896c3-125">Время дня, в которое пользователь заканчивает работать.</span><span class="sxs-lookup"><span data-stu-id="896c3-125">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="896c3-126">timeZone</span><span class="sxs-lookup"><span data-stu-id="896c3-126">timeZone</span></span> | [<span data-ttu-id="896c3-127">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="896c3-127">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="896c3-128">Часовой пояс, к которому относится рабочее время.</span><span class="sxs-lookup"><span data-stu-id="896c3-128">The time zone to which the working hours apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="896c3-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="896c3-129">JSON representation</span></span>

<span data-ttu-id="896c3-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="896c3-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "string (TimeOfDay)",
  "endTime": "string (TimeOfDay)",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


