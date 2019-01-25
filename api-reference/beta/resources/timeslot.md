---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
ms.openlocfilehash: 9a2469447bbf0fbb059b41f9bf2b546c341f9190
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517766"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="6ec60-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="6ec60-103">timeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ec60-104">Период времени.</span><span class="sxs-lookup"><span data-stu-id="6ec60-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ec60-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6ec60-105">JSON representation</span></span>

<span data-ttu-id="6ec60-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6ec60-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="6ec60-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ec60-107">Properties</span></span>
| <span data-ttu-id="6ec60-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ec60-108">Property</span></span>     | <span data-ttu-id="6ec60-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6ec60-109">Type</span></span>   |<span data-ttu-id="6ec60-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ec60-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ec60-111">end</span><span class="sxs-lookup"><span data-stu-id="6ec60-111">end</span></span>|[<span data-ttu-id="6ec60-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6ec60-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6ec60-113">Время начала периода.</span><span class="sxs-lookup"><span data-stu-id="6ec60-113">The time a period begins.</span></span>|
|<span data-ttu-id="6ec60-114">start</span><span class="sxs-lookup"><span data-stu-id="6ec60-114">start</span></span>|[<span data-ttu-id="6ec60-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6ec60-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6ec60-116">Время окончания периода.</span><span class="sxs-lookup"><span data-stu-id="6ec60-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
