---
title: Тип ресурса Букингворкхаурс
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: cfc15d65e840d7634c5c9134c5fc36a244f73286
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507889"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="10de5-104">Тип ресурса Букингворкхаурс</span><span class="sxs-lookup"><span data-stu-id="10de5-104">bookingWorkHours resource type</span></span>

<span data-ttu-id="10de5-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="10de5-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="10de5-106">Представляет набор рабочих часов в один день недели для [букингбусинесс](bookingbusiness.md) или [букингстаффмембер](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="10de5-106">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="10de5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="10de5-107">Properties</span></span>
| <span data-ttu-id="10de5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="10de5-108">Property</span></span>     | <span data-ttu-id="10de5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="10de5-109">Type</span></span>   |<span data-ttu-id="10de5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="10de5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10de5-111">открыт</span><span class="sxs-lookup"><span data-stu-id="10de5-111">day</span></span>|<span data-ttu-id="10de5-112">String</span><span class="sxs-lookup"><span data-stu-id="10de5-112">String</span></span>| <span data-ttu-id="10de5-113">День недели, представленный этим экземпляром.</span><span class="sxs-lookup"><span data-stu-id="10de5-113">The day of the week represented by this instance.</span></span> <span data-ttu-id="10de5-114">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="10de5-114">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="10de5-115">тимеслотс</span><span class="sxs-lookup"><span data-stu-id="10de5-115">timeSlots</span></span>|<span data-ttu-id="10de5-116">Коллекция [букингворктимеслот](bookingworktimeslot.md)</span><span class="sxs-lookup"><span data-stu-id="10de5-116">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="10de5-117">Список начальных и конечных моментов в течение дня.</span><span class="sxs-lookup"><span data-stu-id="10de5-117">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10de5-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10de5-118">JSON representation</span></span>

<span data-ttu-id="10de5-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10de5-119">The following is a JSON representation of the resource.</span></span>

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
