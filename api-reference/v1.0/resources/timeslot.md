---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
ms.openlocfilehash: e01b8d0f34a21eb18bc92e8bcc4e1b8365541d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860566"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="2e7f8-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="2e7f8-103">timeSlot resource type</span></span>

<span data-ttu-id="2e7f8-104">Период времени.</span><span class="sxs-lookup"><span data-stu-id="2e7f8-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e7f8-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2e7f8-105">JSON representation</span></span>

<span data-ttu-id="2e7f8-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="2e7f8-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="2e7f8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e7f8-107">Properties</span></span>
| <span data-ttu-id="2e7f8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e7f8-108">Property</span></span>     | <span data-ttu-id="2e7f8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2e7f8-109">Type</span></span>   |<span data-ttu-id="2e7f8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e7f8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e7f8-111">end</span><span class="sxs-lookup"><span data-stu-id="2e7f8-111">end</span></span>|[<span data-ttu-id="2e7f8-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2e7f8-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2e7f8-113">Время начала периода.</span><span class="sxs-lookup"><span data-stu-id="2e7f8-113">The time a period begins.</span></span>|
|<span data-ttu-id="2e7f8-114">start</span><span class="sxs-lookup"><span data-stu-id="2e7f8-114">start</span></span>|[<span data-ttu-id="2e7f8-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2e7f8-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2e7f8-116">Время окончания периода.</span><span class="sxs-lookup"><span data-stu-id="2e7f8-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
