---
title: Тип ресурса Букингворкхаурс
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 0c6eec989e4c5474115810dfefe6578d7fc5deec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071677"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="66847-104">Тип ресурса Букингворкхаурс</span><span class="sxs-lookup"><span data-stu-id="66847-104">bookingWorkHours resource type</span></span>

<span data-ttu-id="66847-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66847-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="66847-106">Представляет набор рабочих часов в один день недели для [букингбусинесс](bookingbusiness.md) или [букингстаффмембер](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="66847-106">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="66847-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="66847-107">Properties</span></span>
| <span data-ttu-id="66847-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="66847-108">Property</span></span>     | <span data-ttu-id="66847-109">Тип</span><span class="sxs-lookup"><span data-stu-id="66847-109">Type</span></span>   |<span data-ttu-id="66847-110">Описание</span><span class="sxs-lookup"><span data-stu-id="66847-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66847-111">открыт</span><span class="sxs-lookup"><span data-stu-id="66847-111">day</span></span>|<span data-ttu-id="66847-112">String</span><span class="sxs-lookup"><span data-stu-id="66847-112">String</span></span>| <span data-ttu-id="66847-113">День недели, представленный этим экземпляром.</span><span class="sxs-lookup"><span data-stu-id="66847-113">The day of the week represented by this instance.</span></span> <span data-ttu-id="66847-114">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="66847-114">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="66847-115">тимеслотс</span><span class="sxs-lookup"><span data-stu-id="66847-115">timeSlots</span></span>|<span data-ttu-id="66847-116">Коллекция [букингворктимеслот](bookingworktimeslot.md)</span><span class="sxs-lookup"><span data-stu-id="66847-116">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="66847-117">Список начальных и конечных моментов в течение дня.</span><span class="sxs-lookup"><span data-stu-id="66847-117">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66847-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66847-118">JSON representation</span></span>

<span data-ttu-id="66847-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66847-119">The following is a JSON representation of the resource.</span></span>

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


