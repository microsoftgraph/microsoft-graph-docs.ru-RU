---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 930e0ca20bf6b69641aeb0410514ec4ad37d7ee7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341948"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="86e2b-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="86e2b-103">timeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86e2b-104">Представляет интервал времени для собрания.</span><span class="sxs-lookup"><span data-stu-id="86e2b-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="86e2b-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86e2b-105">JSON representation</span></span>

<span data-ttu-id="86e2b-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="86e2b-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="86e2b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="86e2b-107">Properties</span></span>
| <span data-ttu-id="86e2b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="86e2b-108">Property</span></span>     | <span data-ttu-id="86e2b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="86e2b-109">Type</span></span>   |<span data-ttu-id="86e2b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="86e2b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86e2b-111">end</span><span class="sxs-lookup"><span data-stu-id="86e2b-111">end</span></span>|[<span data-ttu-id="86e2b-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="86e2b-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="86e2b-113">Дата, время и часовой пояс, с которого начинается период.</span><span class="sxs-lookup"><span data-stu-id="86e2b-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="86e2b-114">start</span><span class="sxs-lookup"><span data-stu-id="86e2b-114">start</span></span>|[<span data-ttu-id="86e2b-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="86e2b-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="86e2b-116">Дата, время и часовой пояс, в течение которого заканчивается срок.</span><span class="sxs-lookup"><span data-stu-id="86e2b-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
