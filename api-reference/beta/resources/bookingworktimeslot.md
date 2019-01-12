---
title: Тип ресурса bookingWorkTimeSlot
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 33dd856d678d2cf1ba9da2a747c0bd46f2fd4932
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968486"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="bbaeb-104">Тип ресурса bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="bbaeb-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="bbaeb-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bbaeb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbaeb-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbaeb-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="bbaeb-107">Время начала и окончания для работы.</span><span class="sxs-lookup"><span data-stu-id="bbaeb-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="bbaeb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbaeb-108">Properties</span></span>
| <span data-ttu-id="bbaeb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbaeb-109">Property</span></span>     | <span data-ttu-id="bbaeb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bbaeb-110">Type</span></span>   |<span data-ttu-id="bbaeb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bbaeb-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbaeb-112">end</span><span class="sxs-lookup"><span data-stu-id="bbaeb-112">end</span></span>|<span data-ttu-id="bbaeb-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="bbaeb-113">TimeOfDay</span></span>|<span data-ttu-id="bbaeb-114">Время дня, работа начинается.</span><span class="sxs-lookup"><span data-stu-id="bbaeb-114">The time of the day that work starts.</span></span> <span data-ttu-id="bbaeb-115">Например 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="bbaeb-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="bbaeb-116">start</span><span class="sxs-lookup"><span data-stu-id="bbaeb-116">start</span></span>|<span data-ttu-id="bbaeb-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="bbaeb-117">TimeOfDay</span></span>|<span data-ttu-id="bbaeb-118">Время дня, работа останавливается.</span><span class="sxs-lookup"><span data-stu-id="bbaeb-118">The time of the day that work stops.</span></span> <span data-ttu-id="bbaeb-119">Например 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="bbaeb-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbaeb-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbaeb-120">JSON representation</span></span>

<span data-ttu-id="bbaeb-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbaeb-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkTimeSlot"
}-->

```json
{
  "end": "String (timestamp)",
  "start": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
