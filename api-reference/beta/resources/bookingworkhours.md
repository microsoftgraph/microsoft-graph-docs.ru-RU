---
title: Тип ресурса Букингворкхаурс
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 4011dd7f5f363afc4d0017d5b8931cc26e9f20e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974121"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="5dcd5-104">Тип ресурса Букингворкхаурс</span><span class="sxs-lookup"><span data-stu-id="5dcd5-104">bookingWorkHours resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="5dcd5-105">Представляет набор рабочих часов в один день недели для [букингбусинесс](bookingbusiness.md) или [букингстаффмембер](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="5dcd5-105">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5dcd5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5dcd5-106">Properties</span></span>
| <span data-ttu-id="5dcd5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dcd5-107">Property</span></span>     | <span data-ttu-id="5dcd5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5dcd5-108">Type</span></span>   |<span data-ttu-id="5dcd5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5dcd5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dcd5-110">открыт</span><span class="sxs-lookup"><span data-stu-id="5dcd5-110">day</span></span>|<span data-ttu-id="5dcd5-111">String</span><span class="sxs-lookup"><span data-stu-id="5dcd5-111">String</span></span>| <span data-ttu-id="5dcd5-112">День недели, представленный этим экземпляром.</span><span class="sxs-lookup"><span data-stu-id="5dcd5-112">The day of the week represented by this instance.</span></span> <span data-ttu-id="5dcd5-113">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="5dcd5-113">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="5dcd5-114">Тимеслотс</span><span class="sxs-lookup"><span data-stu-id="5dcd5-114">timeSlots</span></span>|<span data-ttu-id="5dcd5-115">Коллекция [букингворктимеслот](bookingworktimeslot.md)</span><span class="sxs-lookup"><span data-stu-id="5dcd5-115">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="5dcd5-116">Список начальных и конечных моментов в течение дня.</span><span class="sxs-lookup"><span data-stu-id="5dcd5-116">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5dcd5-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5dcd5-117">JSON representation</span></span>

<span data-ttu-id="5dcd5-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dcd5-118">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
