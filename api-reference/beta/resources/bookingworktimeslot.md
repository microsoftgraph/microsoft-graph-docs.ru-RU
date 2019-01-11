---
title: Тип ресурса bookingWorkTimeSlot
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 69a802e4addd3c0cb821a630707a62724ea984a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839559"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="37f6c-104">Тип ресурса bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="37f6c-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="37f6c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37f6c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37f6c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37f6c-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="37f6c-107">Время начала и окончания для работы.</span><span class="sxs-lookup"><span data-stu-id="37f6c-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="37f6c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="37f6c-108">Properties</span></span>
| <span data-ttu-id="37f6c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="37f6c-109">Property</span></span>     | <span data-ttu-id="37f6c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="37f6c-110">Type</span></span>   |<span data-ttu-id="37f6c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37f6c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37f6c-112">end</span><span class="sxs-lookup"><span data-stu-id="37f6c-112">end</span></span>|<span data-ttu-id="37f6c-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="37f6c-113">TimeOfDay</span></span>|<span data-ttu-id="37f6c-114">Время дня, работа начинается.</span><span class="sxs-lookup"><span data-stu-id="37f6c-114">The time of the day that work starts.</span></span> <span data-ttu-id="37f6c-115">Например 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="37f6c-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="37f6c-116">start</span><span class="sxs-lookup"><span data-stu-id="37f6c-116">start</span></span>|<span data-ttu-id="37f6c-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="37f6c-117">TimeOfDay</span></span>|<span data-ttu-id="37f6c-118">Время дня, работа останавливается.</span><span class="sxs-lookup"><span data-stu-id="37f6c-118">The time of the day that work stops.</span></span> <span data-ttu-id="37f6c-119">Например 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="37f6c-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37f6c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37f6c-120">JSON representation</span></span>

<span data-ttu-id="37f6c-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37f6c-121">The following is a JSON representation of the resource.</span></span>

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
