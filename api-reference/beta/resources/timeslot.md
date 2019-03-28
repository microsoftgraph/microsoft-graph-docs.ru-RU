---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ee8746d1278f4c9422fa2803895a20c359d5f1e0
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936292"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="3e2aa-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="3e2aa-103">timeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e2aa-104">Представляет интервал времени для собрания.</span><span class="sxs-lookup"><span data-stu-id="3e2aa-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e2aa-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e2aa-105">JSON representation</span></span>

<span data-ttu-id="3e2aa-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3e2aa-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3e2aa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e2aa-107">Properties</span></span>
| <span data-ttu-id="3e2aa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e2aa-108">Property</span></span>     | <span data-ttu-id="3e2aa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3e2aa-109">Type</span></span>   |<span data-ttu-id="3e2aa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3e2aa-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e2aa-111">end</span><span class="sxs-lookup"><span data-stu-id="3e2aa-111">end</span></span>|[<span data-ttu-id="3e2aa-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e2aa-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3e2aa-113">Дата, время и часовой пояс, с которого начинается период.</span><span class="sxs-lookup"><span data-stu-id="3e2aa-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="3e2aa-114">start</span><span class="sxs-lookup"><span data-stu-id="3e2aa-114">start</span></span>|[<span data-ttu-id="3e2aa-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e2aa-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3e2aa-116">Дата, время и часовой пояс, в течение которого заканчивается срок.</span><span class="sxs-lookup"><span data-stu-id="3e2aa-116">The date, time, and time zone that a period ends.</span></span>|

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
