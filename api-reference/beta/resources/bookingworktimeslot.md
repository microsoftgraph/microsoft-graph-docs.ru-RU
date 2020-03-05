---
title: Тип ресурса Букингворктимеслот
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2c9caa1f5a9a2b78911e77df27b84079efd70ab2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507882"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="b835f-104">Тип ресурса Букингворктимеслот</span><span class="sxs-lookup"><span data-stu-id="b835f-104">bookingWorkTimeSlot resource type</span></span>

<span data-ttu-id="b835f-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b835f-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="b835f-106">Время начала и окончания работы.</span><span class="sxs-lookup"><span data-stu-id="b835f-106">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="b835f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b835f-107">Properties</span></span>
| <span data-ttu-id="b835f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b835f-108">Property</span></span>     | <span data-ttu-id="b835f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b835f-109">Type</span></span>   |<span data-ttu-id="b835f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b835f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b835f-111">end</span><span class="sxs-lookup"><span data-stu-id="b835f-111">end</span></span>|<span data-ttu-id="b835f-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b835f-112">TimeOfDay</span></span>|<span data-ttu-id="b835f-113">Время суток, в которое начинается рабочий день.</span><span class="sxs-lookup"><span data-stu-id="b835f-113">The time of the day that work starts.</span></span> <span data-ttu-id="b835f-114">Например, 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="b835f-114">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="b835f-115">start</span><span class="sxs-lookup"><span data-stu-id="b835f-115">start</span></span>|<span data-ttu-id="b835f-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b835f-116">TimeOfDay</span></span>|<span data-ttu-id="b835f-117">Время суток, когда работа завершается.</span><span class="sxs-lookup"><span data-stu-id="b835f-117">The time of the day that work stops.</span></span> <span data-ttu-id="b835f-118">Например, 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="b835f-118">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b835f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b835f-119">JSON representation</span></span>

<span data-ttu-id="b835f-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b835f-120">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
