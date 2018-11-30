---
title: Тип ресурсов timeSlot
description: Период времени.
ms.openlocfilehash: 43ce20e006f2a6946877a4ffd2bf730d45d6d1c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026414"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="b36aa-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="b36aa-103">timeSlot resource type</span></span>

<span data-ttu-id="b36aa-104">Период времени.</span><span class="sxs-lookup"><span data-stu-id="b36aa-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b36aa-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b36aa-105">JSON representation</span></span>

<span data-ttu-id="b36aa-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b36aa-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b36aa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b36aa-107">Properties</span></span>
| <span data-ttu-id="b36aa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b36aa-108">Property</span></span>     | <span data-ttu-id="b36aa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b36aa-109">Type</span></span>   |<span data-ttu-id="b36aa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b36aa-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b36aa-111">end</span><span class="sxs-lookup"><span data-stu-id="b36aa-111">end</span></span>|[<span data-ttu-id="b36aa-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b36aa-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b36aa-113">Время начала периода.</span><span class="sxs-lookup"><span data-stu-id="b36aa-113">The time a period begins.</span></span>|
|<span data-ttu-id="b36aa-114">start</span><span class="sxs-lookup"><span data-stu-id="b36aa-114">start</span></span>|[<span data-ttu-id="b36aa-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b36aa-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b36aa-116">Время окончания периода.</span><span class="sxs-lookup"><span data-stu-id="b36aa-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->