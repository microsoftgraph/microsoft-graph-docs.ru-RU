---
title: Тип ресурсов timeSlot
description: Период времени.
ms.openlocfilehash: c1df6ea458bf6742dc20149e62d9760a8a6510e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081473"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="14807-103">Тип ресурсов timeSlot</span><span class="sxs-lookup"><span data-stu-id="14807-103">timeSlot resource type</span></span>

> <span data-ttu-id="14807-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="14807-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14807-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14807-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14807-106">Период времени.</span><span class="sxs-lookup"><span data-stu-id="14807-106">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14807-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="14807-107">JSON representation</span></span>

<span data-ttu-id="14807-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="14807-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="14807-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="14807-109">Properties</span></span>
| <span data-ttu-id="14807-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="14807-110">Property</span></span>     | <span data-ttu-id="14807-111">Тип</span><span class="sxs-lookup"><span data-stu-id="14807-111">Type</span></span>   |<span data-ttu-id="14807-112">Описание</span><span class="sxs-lookup"><span data-stu-id="14807-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14807-113">end</span><span class="sxs-lookup"><span data-stu-id="14807-113">end</span></span>|[<span data-ttu-id="14807-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="14807-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="14807-115">Время начала периода.</span><span class="sxs-lookup"><span data-stu-id="14807-115">The time a period begins.</span></span>|
|<span data-ttu-id="14807-116">start</span><span class="sxs-lookup"><span data-stu-id="14807-116">start</span></span>|[<span data-ttu-id="14807-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="14807-117">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="14807-118">Время окончания периода.</span><span class="sxs-lookup"><span data-stu-id="14807-118">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->