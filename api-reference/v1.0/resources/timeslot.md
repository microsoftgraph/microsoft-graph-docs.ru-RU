---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7b09ae7f1c60a8348e9f22b856c65f326432e408
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936243"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="6898f-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="6898f-103">timeSlot resource type</span></span>

<span data-ttu-id="6898f-104">Представляет интервал времени для собрания.</span><span class="sxs-lookup"><span data-stu-id="6898f-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6898f-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6898f-105">JSON representation</span></span>

<span data-ttu-id="6898f-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6898f-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6898f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6898f-107">Properties</span></span>
| <span data-ttu-id="6898f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6898f-108">Property</span></span>     | <span data-ttu-id="6898f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6898f-109">Type</span></span>   |<span data-ttu-id="6898f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6898f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6898f-111">end</span><span class="sxs-lookup"><span data-stu-id="6898f-111">end</span></span>|[<span data-ttu-id="6898f-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6898f-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6898f-113">Дата, время и часовой пояс, с которого начинается период.</span><span class="sxs-lookup"><span data-stu-id="6898f-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="6898f-114">start</span><span class="sxs-lookup"><span data-stu-id="6898f-114">start</span></span>|[<span data-ttu-id="6898f-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6898f-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6898f-116">Дата, время и часовой пояс, в течение которого заканчивается срок.</span><span class="sxs-lookup"><span data-stu-id="6898f-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
