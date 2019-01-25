---
title: Тип ресурса bookingWorkTimeSlot
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a193843617d5acc7e18d8a06993a1629b80762be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513790"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="b66e5-104">Тип ресурса bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="b66e5-104">bookingWorkTimeSlot resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="b66e5-105">Время начала и окончания для работы.</span><span class="sxs-lookup"><span data-stu-id="b66e5-105">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="b66e5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b66e5-106">Properties</span></span>
| <span data-ttu-id="b66e5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b66e5-107">Property</span></span>     | <span data-ttu-id="b66e5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b66e5-108">Type</span></span>   |<span data-ttu-id="b66e5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b66e5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b66e5-110">end</span><span class="sxs-lookup"><span data-stu-id="b66e5-110">end</span></span>|<span data-ttu-id="b66e5-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b66e5-111">TimeOfDay</span></span>|<span data-ttu-id="b66e5-112">Время дня, работа начинается.</span><span class="sxs-lookup"><span data-stu-id="b66e5-112">The time of the day that work starts.</span></span> <span data-ttu-id="b66e5-113">Например 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="b66e5-113">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="b66e5-114">start</span><span class="sxs-lookup"><span data-stu-id="b66e5-114">start</span></span>|<span data-ttu-id="b66e5-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b66e5-115">TimeOfDay</span></span>|<span data-ttu-id="b66e5-116">Время дня, работа останавливается.</span><span class="sxs-lookup"><span data-stu-id="b66e5-116">The time of the day that work stops.</span></span> <span data-ttu-id="b66e5-117">Например 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="b66e5-117">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b66e5-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b66e5-118">JSON representation</span></span>

<span data-ttu-id="b66e5-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b66e5-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingworktimeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
