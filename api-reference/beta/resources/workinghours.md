---
title: Тип ресурса workingHours
description: Представляет дни недели и часы работы пользователя в определенном часовом поясе.
localization_priority: Normal
ms.openlocfilehash: 40a74cd1446dc2553e30ebd0616b0b0e33192778
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512285"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="95b02-103">Тип ресурса workingHours</span><span class="sxs-lookup"><span data-stu-id="95b02-103">workingHours resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95b02-104">Представляет дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="95b02-104">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="95b02-105">Доступ к рабочему времени пользователя полезен в тех случаях, когда требуется планировать действия или ресурсы.</span><span class="sxs-lookup"><span data-stu-id="95b02-105">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="95b02-106">Вы можете [получать](../api/user-get-mailboxsettings.md#request-3) и [задавать](../api/user-update-mailboxsettings.md#request-2) рабочее время пользователя в [параметрах его почтового ящика](mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="95b02-106">You can [get](../api/user-get-mailboxsettings.md#request-3) and [set](../api/user-update-mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="95b02-107">Вы можете задать часовой пояс для своего рабочего времени отдельно от часового пояса, заданного для клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="95b02-107">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="95b02-108">Например, это может быть полезно, если вы перемещаетесь в другой часовой пояс, где вы обычно не работаете.</span><span class="sxs-lookup"><span data-stu-id="95b02-108">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="95b02-109">Для клиента Outlook</span><span class="sxs-lookup"><span data-stu-id="95b02-109">You can set the Outlook client</span></span>  
<span data-ttu-id="95b02-110">можно задать целевой часовой пояс, чтобы значения времени в Outlook соответствовали местному времени, пока вы там находитесь.</span><span class="sxs-lookup"><span data-stu-id="95b02-110">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="95b02-111">Когда другие люди запрашивают рабочие встречи с вами на вашем обычном рабочем месте, они по-прежнему могут учитывать ваше рабочее время в соответствующем часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="95b02-111">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="95b02-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="95b02-112">Properties</span></span>
| <span data-ttu-id="95b02-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="95b02-113">Property</span></span>     | <span data-ttu-id="95b02-114">Тип</span><span class="sxs-lookup"><span data-stu-id="95b02-114">Type</span></span>   |<span data-ttu-id="95b02-115">Описание</span><span class="sxs-lookup"><span data-stu-id="95b02-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95b02-116">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="95b02-116">daysOfWeek</span></span> | <span data-ttu-id="95b02-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="95b02-117">String collection</span></span> | <span data-ttu-id="95b02-118">Дни недели, в которые работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="95b02-118">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="95b02-119">startTime</span><span class="sxs-lookup"><span data-stu-id="95b02-119">startTime</span></span> | <span data-ttu-id="95b02-120">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="95b02-120">Edm.TimeOfDay</span></span> | <span data-ttu-id="95b02-121">Время дня, в которое пользователь начинает работать.</span><span class="sxs-lookup"><span data-stu-id="95b02-121">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="95b02-122">endTime</span><span class="sxs-lookup"><span data-stu-id="95b02-122">endTime</span></span> | <span data-ttu-id="95b02-123">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="95b02-123">Edm.TimeOfDay</span></span> | <span data-ttu-id="95b02-124">Время дня, в которое пользователь заканчивает работать.</span><span class="sxs-lookup"><span data-stu-id="95b02-124">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="95b02-125">timeZone</span><span class="sxs-lookup"><span data-stu-id="95b02-125">timeZone</span></span> | [<span data-ttu-id="95b02-126">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="95b02-126">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="95b02-127">Часовой пояс, к которому относится рабочее время.</span><span class="sxs-lookup"><span data-stu-id="95b02-127">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="95b02-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95b02-128">JSON representation</span></span>

<span data-ttu-id="95b02-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95b02-129">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/workinghours.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
