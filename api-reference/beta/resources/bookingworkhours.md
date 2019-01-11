---
title: Тип ресурса bookingWorkHours
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 94920287cd7358c68686da2d0969c676e3c481ee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888958"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="21ab6-104">Тип ресурса bookingWorkHours</span><span class="sxs-lookup"><span data-stu-id="21ab6-104">bookingWorkHours resource type</span></span>

 > <span data-ttu-id="21ab6-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="21ab6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21ab6-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21ab6-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="21ab6-107">Представляет набор рабочих часов в один день недели для [bookingBusiness](bookingbusiness.md) или [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="21ab6-107">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="21ab6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="21ab6-108">Properties</span></span>
| <span data-ttu-id="21ab6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="21ab6-109">Property</span></span>     | <span data-ttu-id="21ab6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="21ab6-110">Type</span></span>   |<span data-ttu-id="21ab6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21ab6-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21ab6-112">день</span><span class="sxs-lookup"><span data-stu-id="21ab6-112">day</span></span>|<span data-ttu-id="21ab6-113">Строка</span><span class="sxs-lookup"><span data-stu-id="21ab6-113">String</span></span>| <span data-ttu-id="21ab6-114">День недели, представленный в этом экземпляре.</span><span class="sxs-lookup"><span data-stu-id="21ab6-114">The day of the week represented by this instance.</span></span> <span data-ttu-id="21ab6-115">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="21ab6-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="21ab6-116">таймслоты</span><span class="sxs-lookup"><span data-stu-id="21ab6-116">timeSlots</span></span>|<span data-ttu-id="21ab6-117">[bookingWorkTimeSlot](bookingworktimeslot.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="21ab6-117">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="21ab6-118">Список времени начала и окончания во время дня.</span><span class="sxs-lookup"><span data-stu-id="21ab6-118">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21ab6-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21ab6-119">JSON representation</span></span>

<span data-ttu-id="21ab6-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21ab6-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkHours"
}-->

```json
{
  "day": "String",
  "timeSlots": [{"@odata.type": "microsoft.graph.bookingWorkTimeSlot"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
