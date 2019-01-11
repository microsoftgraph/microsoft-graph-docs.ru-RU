---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
ms.openlocfilehash: 1f383a7feafbb3816ef838d8f0667eebdd42443f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877933"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="e3de3-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="e3de3-103">timeSlot resource type</span></span>

> <span data-ttu-id="e3de3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3de3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3de3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3de3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3de3-106">Период времени.</span><span class="sxs-lookup"><span data-stu-id="e3de3-106">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3de3-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3de3-107">JSON representation</span></span>

<span data-ttu-id="e3de3-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e3de3-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="e3de3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3de3-109">Properties</span></span>
| <span data-ttu-id="e3de3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3de3-110">Property</span></span>     | <span data-ttu-id="e3de3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e3de3-111">Type</span></span>   |<span data-ttu-id="e3de3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e3de3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3de3-113">end</span><span class="sxs-lookup"><span data-stu-id="e3de3-113">end</span></span>|[<span data-ttu-id="e3de3-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e3de3-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e3de3-115">Время начала периода.</span><span class="sxs-lookup"><span data-stu-id="e3de3-115">The time a period begins.</span></span>|
|<span data-ttu-id="e3de3-116">start</span><span class="sxs-lookup"><span data-stu-id="e3de3-116">start</span></span>|[<span data-ttu-id="e3de3-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e3de3-117">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="e3de3-118">Время окончания периода.</span><span class="sxs-lookup"><span data-stu-id="e3de3-118">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
