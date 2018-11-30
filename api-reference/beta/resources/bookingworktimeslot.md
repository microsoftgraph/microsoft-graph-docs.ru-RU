---
title: Тип ресурса bookingWorkTimeSlot
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 61436ca3e94ab15c44fc1898827a3de511c8ee94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077752"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="f356e-104">Тип ресурса bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="f356e-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="f356e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f356e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f356e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f356e-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f356e-107">Время начала и окончания для работы.</span><span class="sxs-lookup"><span data-stu-id="f356e-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="f356e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f356e-108">Properties</span></span>
| <span data-ttu-id="f356e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f356e-109">Property</span></span>     | <span data-ttu-id="f356e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f356e-110">Type</span></span>   |<span data-ttu-id="f356e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f356e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f356e-112">end</span><span class="sxs-lookup"><span data-stu-id="f356e-112">end</span></span>|<span data-ttu-id="f356e-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f356e-113">TimeOfDay</span></span>|<span data-ttu-id="f356e-114">Время дня, работа начинается.</span><span class="sxs-lookup"><span data-stu-id="f356e-114">The time of the day that work starts.</span></span> <span data-ttu-id="f356e-115">Например 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="f356e-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="f356e-116">start</span><span class="sxs-lookup"><span data-stu-id="f356e-116">start</span></span>|<span data-ttu-id="f356e-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f356e-117">TimeOfDay</span></span>|<span data-ttu-id="f356e-118">Время дня, работа останавливается.</span><span class="sxs-lookup"><span data-stu-id="f356e-118">The time of the day that work stops.</span></span> <span data-ttu-id="f356e-119">Например 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="f356e-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f356e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f356e-120">JSON representation</span></span>

<span data-ttu-id="f356e-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f356e-121">The following is a JSON representation of the resource.</span></span>

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