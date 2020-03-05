---
title: Тип ресурса workingHours
description: Представляет дни недели и часы работы пользователя в определенном часовом поясе.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 67a61c5ca767f00c32bf568cea4e495d5b0909ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519073"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="c088a-103">Тип ресурса workingHours</span><span class="sxs-lookup"><span data-stu-id="c088a-103">workingHours resource type</span></span>

<span data-ttu-id="c088a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c088a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c088a-105">Представляет дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="c088a-105">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="c088a-106">Доступ к рабочему времени пользователя полезен в тех случаях, когда требуется планировать действия или ресурсы.</span><span class="sxs-lookup"><span data-stu-id="c088a-106">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="c088a-107">Вы можете [получать](../api/user-get-mailboxsettings.md#example-3) и [задавать](../api/user-update-mailboxsettings.md#example-2) рабочее время пользователя в [параметрах его почтового ящика](mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="c088a-107">You can [get](../api/user-get-mailboxsettings.md#example-3) and [set](../api/user-update-mailboxsettings.md#example-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="c088a-108">Вы можете задать часовой пояс для своего рабочего времени отдельно от часового пояса, заданного для клиента Outlook.</span><span class="sxs-lookup"><span data-stu-id="c088a-108">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="c088a-109">Например, это может быть полезно, если вы перемещаетесь в другой часовой пояс, где вы обычно не работаете.</span><span class="sxs-lookup"><span data-stu-id="c088a-109">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="c088a-110">Для клиента Outlook</span><span class="sxs-lookup"><span data-stu-id="c088a-110">You can set the Outlook client</span></span>  
<span data-ttu-id="c088a-111">можно задать целевой часовой пояс, чтобы значения времени в Outlook соответствовали местному времени, пока вы там находитесь.</span><span class="sxs-lookup"><span data-stu-id="c088a-111">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="c088a-112">Когда другие люди запрашивают рабочие встречи с вами на вашем обычном рабочем месте, они по-прежнему могут учитывать ваше рабочее время в соответствующем часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="c088a-112">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="c088a-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="c088a-113">Properties</span></span>
| <span data-ttu-id="c088a-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="c088a-114">Property</span></span>     | <span data-ttu-id="c088a-115">Тип</span><span class="sxs-lookup"><span data-stu-id="c088a-115">Type</span></span>   |<span data-ttu-id="c088a-116">Описание</span><span class="sxs-lookup"><span data-stu-id="c088a-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c088a-117">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="c088a-117">daysOfWeek</span></span> | <span data-ttu-id="c088a-118">Коллекция dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="c088a-118">dayOfWeek collection</span></span> | <span data-ttu-id="c088a-119">Дни недели, в которые работает пользователь.</span><span class="sxs-lookup"><span data-stu-id="c088a-119">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="c088a-120">startTime</span><span class="sxs-lookup"><span data-stu-id="c088a-120">startTime</span></span> | <span data-ttu-id="c088a-121">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c088a-121">Edm.TimeOfDay</span></span> | <span data-ttu-id="c088a-122">Время дня, в которое пользователь начинает работать.</span><span class="sxs-lookup"><span data-stu-id="c088a-122">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="c088a-123">endTime</span><span class="sxs-lookup"><span data-stu-id="c088a-123">endTime</span></span> | <span data-ttu-id="c088a-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c088a-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="c088a-125">Время дня, в которое пользователь заканчивает работать.</span><span class="sxs-lookup"><span data-stu-id="c088a-125">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="c088a-126">timeZone</span><span class="sxs-lookup"><span data-stu-id="c088a-126">timeZone</span></span> | [<span data-ttu-id="c088a-127">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="c088a-127">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="c088a-128">Часовой пояс, к которому относится рабочее время.</span><span class="sxs-lookup"><span data-stu-id="c088a-128">The time zone to which the working hours apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c088a-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c088a-129">JSON representation</span></span>

<span data-ttu-id="c088a-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c088a-130">Here is a JSON representation of the resource.</span></span>

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
